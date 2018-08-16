---
order: 5
title:
  zh-CN: 竖直方向的小型步骤条
  en-US: عمودی ورژن کوچک
---

## zh-CN

简单的竖直方向的小型步骤条。

## en-US

A simple mini version step bar in the vertical direction.

````jsx
import { Steps } from 'antd';
const Step = Steps.Step;

ReactDOM.render(
  <Steps direction="vertical" size="small" current={1}>
    <Step title="تمام شده" description="توضیح." />
    <Step title="در حال بررسی" description="توضیح." />
    <Step title="صبر کنید" description="توضیح." />
  </Steps>, mountNode);
````
