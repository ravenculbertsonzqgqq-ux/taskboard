# taskboard · 任务台入口

这是「任务台」的稳定入口页：一个 GitHub Pages 静态页，会读取仓库中的 `link.json` 并跳转到**当前生效**的公网隧道地址。

- `index.html`：自动跳转页（纯静态，不收集任何信息，不索要凭据）
- `link.json`：当前公网隧道地址与更新时间

注意：GitHub Pages 只能托管静态文件，任务台本体（Python 后端）运行在自有机器上，通过 cloudflared quick tunnel 暴露；隧道每次重启域名都会变化，届时需要更新 `link.json`。

登录任务台需要账号密码，请向站长索取。本页与任务台页面均不会向你请求其他信息。
