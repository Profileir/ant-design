---
order: 2
title:
  zh-CN: 带图标的步骤条
  en-US: همراه آیکون
---

## zh-CN

通过设置 `Steps.Step` 的 `icon` 属性，可以启用自定义图标。

## en-US

You can use your own custom icons by setting the property `icon` for `Steps.Step`.

````jsx
import { Steps, Icon } from 'antd';
const Step = Steps.Step;

ReactDOM.render(
  <Steps>
    <Step status="finish" title="ورود" icon={<Icon type="user" />} />
    <Step status="finish" title="تایید" icon={<Icon type="solution" />} />
    <Step status="process" title="پرداخت" icon={<Icon type="loading" />} />
    <Step status="wait" title="انجام شد" icon={<Icon type="smile-o" />} />
  </Steps>, mountNode);
````
