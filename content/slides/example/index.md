---
title: IoT Energy Services Composition
summary: An overview of Energy-as-a-Service (EaaS) in the IoT context.
authors: 
- admin
tags: [IoT, Energy]
categories: [Energy Services]
date: "2023-04-07"
slides:
  # Choose a theme from https://github.com/hakimel/reveal.js#theming
  theme: black
  # Choose a code highlighting style (if highlighting enabled in `params.toml`)
  #   Light style: github. Dark style: dracula (default).
  highlight_style: dracula
---

# IoT Energy Services Composition

---
## Energy Harvesting
Problem formulation

$$
\begin{aligned}
head_i = \mathbf{Softmax}\left(\frac{(h^t)^T\overline{W}^Q_i(h^t)^TW^{K^T}_i}{\sqrt{d}}\right)(h^t)^TW^V_i \\
\mu_{\mathcal{B}} \leftarrow \frac{1}{m} \sum^{m}_{i} x_{i} \\
\sigma^{2}_{\mathcal{B}} \leftarrow \frac{1}{m} \sum^{m}_{i}(x_{i}-\mu_{\mathcal{B}})^{2}\\
\hat{x}_{i} \leftarrow \frac{x_{i}-\mu_{\mathcal{B}}}{\sqrt{\sigma^{2}_{\mathcal{B}}+\epsilon}}\\
\end{aligned}
$$

---
## EIT Code Demonstration
```python
# decoder input
if self.args.padding == 0:
    dec_inp_zero = torch.zeros([batch_y.shape[0], self.args.pred_len, (batch_y.shape[-1]-1)]).float()
    dec_inp = torch.cat((batch_y[:,self.args.label_len:self.args.label_len+self.args.pred_len,:1],dec_inp_zero), dim=2)
elif self.args.padding == 1:
    dec_inp_one = torch.ones([batch_y.shape[0], self.args.pred_len, batch_y.shape[-1]]).float()
    dec_inp = torch.cat((batch_y[:,self.args.label_len:self.args.label_len+self.args.pred_len,:1],dec_inp_one), dim=2)
dec_inp = torch.cat([batch_y[:, :self.args.label_len, :], dec_inp], dim=1).float().to(self.device)
# encoder - decoder
if self.args.use_amp:
    with torch.cuda.amp.autocast():
        if self.args.output_attention:
            outputs = self.model(batch_x, batch_x_mark, dec_inp, batch_y_mark)[0]
        else:
            outputs = self.model(batch_x, batch_x_mark, dec_inp, batch_y_mark)
else:
    if self.args.output_attention:
        outputs = self.model(batch_x, batch_x_mark, dec_inp, batch_y_mark)[0]
    else:
        outputs = self.model(batch_x, batch_x_mark, dec_inp, batch_y_mark)
```

---
## Energy-as-a-Service (EaaS)

- Energy sharing service
- Transferring wireless energy among IoT devices
- Service paradigm

---

## Energy Provider

- A thing that can share energy
- Owned by users

---

## Energy Consumer

- A thing that requires energy
- Owned by users

---

# Questions?

[Ask](https://github.com/Pengwei-Yang/Pengwei-Yang/discussions)

