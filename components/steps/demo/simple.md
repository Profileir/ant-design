---
order: 0
title:
  zh-CN: 基本用法
  en-US: اولیه
---

## zh-CN

简单的步骤条。

## en-US

The most basic step bar.

````jsx
import { Steps } from 'antd';
const Step = Steps.Step;

ReactDOM.render(
  <Steps current={1}>
    <Step title="تمام شده" description="توضیح." />
    <Step title="در حال بررسی" description="توضیح." />
    <Step title="صبر کنید" description="توضیح." />
  </Steps>, mountNode);
````
