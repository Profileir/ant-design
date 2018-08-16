---
order: 8
title:
  zh-CN: 点状步骤条
  en-US: Dot Style
---

## zh-CN

包含步骤点的进度条。

## en-US

Steps with progress dot style.

````jsx
import { Steps } from 'antd';
const Step = Steps.Step;

ReactDOM.render(
  <Steps progressDot current={1}>
    <Step title="تمام شده" description="توضیح." />
    <Step title="در حال بررسی" description="توضیح." />
    <Step title="صبر کنید" description="توضیح." />
  </Steps>, mountNode);
````
