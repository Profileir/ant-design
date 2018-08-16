---
order: 9
title:
  zh-CN: 自定义点状步骤条
  en-US: شخصی سازی کردن استایل دات‌ها
---

## zh-CN

为点状步骤条增加自定义展示。

## en-US

You can customize the display for Steps with progress dot style.

````jsx
import { Steps, Popover } from 'antd';
const Step = Steps.Step;

const customDot = (dot, { status, index }) => (
  <Popover content={<span>step {index} status: {status}</span>}>
    {dot}
  </Popover>
);

ReactDOM.render(
  <Steps current={1} progressDot={customDot}>
    <Step title="تمام شده" description="هاور کنید." />
    <Step title="در حال بررسی" description="هاور کنید." />
    <Step title="صبر کنید" description="هاور کنید." />
    <Step title="صبر کنید" description="هاور کنید." />
  </Steps>, mountNode);
````
