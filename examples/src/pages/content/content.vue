<template>
    <Page>
        <Header>
            <Navbar>
                <Title ref="title">Content</Title>
            </Navbar>
        </Header>
        <Content class="outer-content">
            <div padding>
                <h5>简介</h5>
                <p>
                    Content组件是Vimo的基础布局组件, 属于三明治结构的中间层, 承接业务展示的部分. 其中, Header/Footer分别为基础布局的头和尾.
                </p>
                <p>
                    Content组件使用的原生scroll, 因此对组件监听: onScroll/onScrollStart/onScrollEnd 这三个事件
                    可以定制业务务求.
                </p>
            </div>
            <List>
                <ListHeader>Character</ListHeader>
                <Item detail-push :to="{name:'contentContext'}">文本</Item>
                <Item detail-push :to="{name:'contentFixed'}">内容固定</Item>
                <Item detail-push :to="{name:'contentFullscreen'}">全屏模式</Item>
                <Item detail-push :to="{name:'contentHideBars'}">隐藏头尾Bar</Item>
                <Item detail-push :to="{name:'contentSetBarStyle'}">设置Bar的样式</Item>
                <Item detail-push :to="{name:'contentScroll'}">滚动监听</Item>
            </List>
        </Content>
    </Page>
</template>
<style scoped lang="scss"></style>
<script type="text/javascript">
  export default{
    data () {
      return {}
    },
    components: {
    },
    mounted () {}
  }
</script>
