<template>
  <div>
    <header class="navbar-wrapper">
      <div class="navbar navbar-fixed-top">
        <div class="container-fluid cl">
          <a class="logo navbar-logo f-l mr-10 hidden-xs">Freegou</a>
          <a class="logo navbar-logo-m f-l mr-10 visible-xs">Freegou</a>
          <span class="logo navbar-slogan f-l mr-10 hidden-xs">v1.0</span>
          <a aria-hidden="false" class="nav-toggle Hui-iconfont visible-xs" href="javascript:;">&#xe667;</a>
          <nav class="nav navbar-nav">
            <ul class="cl">
              <li class="dropDown dropDown_hover"><a href="javascript:;" class="dropDown_A"><i class="Hui-iconfont">&#xe600;</i> 新增 <i class="Hui-iconfont">&#xe6d5;</i></a>
                <ul class="dropDown-menu menu radius box-shadow">
                  <li><a href="javascript:;" onclick="article_add('添加资讯','article-add.html')"><i class="Hui-iconfont">&#xe616;</i> 资讯</a></li>
                  <li><a href="javascript:;" onclick="picture_add('添加资讯','picture-add.html')"><i class="Hui-iconfont">&#xe613;</i> 图片</a></li>
                  <li><a href="javascript:;" onclick="product_add('添加资讯','product-add.html')"><i class="Hui-iconfont">&#xe620;</i> 产品</a></li>
                  <li><a href="javascript:;" onclick="member_add('添加用户','member-add.html','','510')"><i class="Hui-iconfont">&#xe60d;</i> 用户</a></li>
                </ul>
              </li>
            </ul>
          </nav>
          <nav id="Hui-userbar" class="nav navbar-nav navbar-userbar hidden-xs">
            <ul class="cl">
              <li>超级管理员</li>
              <li class="dropDown dropDown_hover"> <a href="#" class="dropDown_A">admin <i class="Hui-iconfont">&#xe6d5;</i></a>
                <ul class="dropDown-menu menu radius box-shadow">
                  <li><a href="javascript:;" onClick="myselfinfo()">个人信息</a></li>
                  <li><a href="#">切换账户</a></li>
                  <li><a href="#">退出</a></li>
                </ul>
              </li>
              <li id="Hui-skin" class="dropDown right dropDown_hover"> <a href="javascript:;" class="dropDown_A" title="换肤"><i class="Hui-iconfont" style="font-size:18px">&#xe62a;</i></a>
                <ul class="dropDown-menu menu radius box-shadow">
                  <li><a href="javascript:;" data-val="default" title="默认（黑色）">默认（黑色）</a></li>
                  <li><a href="javascript:;" data-val="blue" title="蓝色">蓝色</a></li>
                  <li><a href="javascript:;" data-val="green" title="绿色">绿色</a></li>
                  <li><a href="javascript:;" data-val="red" title="红色">红色</a></li>
                  <li><a href="javascript:;" data-val="yellow" title="黄色">黄色</a></li>
                  <li><a href="javascript:;" data-val="orange" title="橙色">橙色</a></li>
                </ul>
              </li>
            </ul>
          </nav>
        </div>
      </div>
    </header>
    <aside class="Hui-aside">

      <div class="menu_dropdown bk_2">
        <dl id="menu-picture">
          <dt><i class="Hui-iconfont">&#xe625;</i> 售货机管理<i class="Hui-iconfont menu_dropdown-arrow">&#xe6d5;</i></dt>
          <dd>
            <ul>
              <li><router-link to="/nav/map" title="位置管理">位置管理</router-link></li>
              <li><router-link to="/nav/shoplist" title="机器列表">机器列表</router-link></li>
            </ul>
          </dd>
        </dl>
        <dl id="menu-product">
          <dt><i class="Hui-iconfont">&#xe620;</i> 商品管理<i class="Hui-iconfont menu_dropdown-arrow">&#xe6d5;</i></dt>
          <dd>
            <ul>
              <li><router-link to="/nav/category" title="分类管理">分类管理</router-link></li>
              <li><router-link to="/nav/product" title="商品列表">商品列表</router-link></li>
            </ul>
          </dd>
        </dl>
        <dl id="menu-admin">
          <dt><i class="Hui-iconfont">&#xe62d;</i> 管理员管理<i class="Hui-iconfont menu_dropdown-arrow">&#xe6d5;</i></dt>
          <dd>
            <ul>
              <li><li><router-link to="/nav/admin" title="管理员列表">管理员列表</router-link></li></li>
            </ul>
          </dd>
        </dl>
        <dl id="menu-tongji">
          <dt><i class="Hui-iconfont">&#xe61a;</i> 系统统计<i class="Hui-iconfont menu_dropdown-arrow">&#xe6d5;</i></dt>
          <dd>
            <ul>
              <li><a href="charts-1.html" title="折线图">折线图</a></li>
              <li><a href="charts-2.html" title="时间轴折线图">时间轴折线图</a></li>
              <li><a href="charts-3.html" title="区域图">区域图</a></li>
              <li><a href="charts-4.html" title="柱状图">柱状图</a></li>
              <li><a href="charts-5.html" title="饼状图">饼状图</a></li>
              <li><a href="charts-6.html" title="3D柱状图">3D柱状图</a></li>
              <li><a href="charts-7.html" title="3D饼状图">3D饼状图</a></li>
            </ul>
          </dd>
        </dl>
        <dl id="menu-system">
          <dt><i class="Hui-iconfont">&#xe62e;</i> 系统管理<i class="Hui-iconfont menu_dropdown-arrow">&#xe6d5;</i></dt>
          <dd>
            <ul>
              <li><a href="system-base.html" title="系统设置">系统设置</a></li>
              <li><a href="system-category.html" title="栏目管理">栏目管理</a></li>
              <li><a href="system-data.html" title="数据字典">数据字典</a></li>
              <li><a href="system-shielding.html" title="屏蔽词">屏蔽词</a></li>
              <li><a href="system-log.html" title="系统日志">系统日志</a></li>
            </ul>
          </dd>
        </dl>
      </div>
    </aside>
    <div class="dislpayArrow hidden-xs"><a class="pngfix" href="javascript:void(0);" onClick="displaynavbar(this)"></a></div>
    <router-view></router-view>
  </div>
</template>
<script>
export default {
  name: 'navigation'
}
</script>
