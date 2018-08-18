---
order: 1
title:
  en-US: JSX style API
  zh-CN: JSX 风格的 API
---

## zh-CN

使用 JSX 风格的 API（2.5.0 以后引入）

> 这个只是一个描述 `columns` 的语法糖，所以你不能用其他组件去包裹 `Column` 和 `ColumnGroup`。

## en-US

Using JSX style API (introduced in 2.5.0)

> Since this is just a syntax sugar for the prop `columns`, you can't compose `Column` and `ColumnGroup` with other Components.

````jsx
import { Table, Icon, Divider } from 'antd';

const { Column, ColumnGroup } = Table;

const data = [{
  key: '1',
  firstName: 'John',
  lastName: 'Brown',
  age: 32,
  address: 'New York No. 1 Lake Park',
}, {
  key: '2',
  firstName: 'Jim',
  lastName: 'Green',
  age: 42,
  address: 'London No. 1 Lake Park',
}, {
  key: '3',
  firstName: 'Joe',
  lastName: 'Black',
  age: 32,
  address: 'Sidney No. 1 Lake Park',
}];

ReactDOM.render(
  <Table dataSource={data}>
    <ColumnGroup title="نام">
      <Column
        title="نام"
        dataIndex="firstName"
        key="firstName"
      />
      <Column
        title="نام خانوادگی"
        dataIndex="lastName"
        key="lastName"
      />
    </ColumnGroup>
    <Column
      title="سن"
      dataIndex="age"
      key="age"
    />
    <Column
      title="آدرس"
      dataIndex="address"
      key="address"
    />
    <Column
      title="عملیات"
      key="action"
      render={(text, record) => (
        <span>
          <a href="javascript:;">عملیات 一 {record.name}</a>
          <Divider type="vertical" />
          <a href="javascript:;">حذف</a>
          <Divider type="vertical" />
          <a href="javascript:;" className="ant-dropdown-link">
            عملیات بیشتر <Icon type="down" />
          </a>
        </span>
      )}
    />
  </Table>, mountNode);
````
