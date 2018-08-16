---
order: 1
title:
  zh-CN: 迷你版
  en-US: ورژن مینی
---

## zh-CN

迷你版的步骤条，通过设置 `<Steps size="small">` 启用.

## en-US

By setting like this: `<Steps size="small">`, you can get a mini version.

````jsx
import { Steps } from 'antd';
const Step = Steps.Step;

ReactDOM.render(
  <Steps size="small" current={1}>
    <Step title="تمام شده" />
    <Step title="در حال بررسی" />
    <Step title="صبر کنید" />
  </Steps>, mountNode);
````
