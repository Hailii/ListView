# 实验三
## UI组件
### Android ListView
![无法显示](/images/1.png)
#### 关键代码
```
创建适配器
SimpleAdapter simpleAdapter=new SimpleAdapter(
                MainActivity.this,
                list_map,
                R.layout.list_items,
                new String[]{"pic","name"},
                new int[]{R.id.items_imageView1,R.id.items_textView1}
        );
        listView.setAdapter(simpleAdapter);
        listView.setOnItemClickListener(new AdapterView.OnItemClickListener() {
            public void onItemClick(AdapterView parent, View view, int position, long id) {
                Toast.makeText(MainActivity.this, name[position], Toast.LENGTH_LONG).show();
            }
        });
```        
