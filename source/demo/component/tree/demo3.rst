.. currentmodule:: tree

从已有的html结构生成树
======================================





Class
-----------------------------------------------

  * :class:`Tree.Node <tree.Node>`
  * :class:`Tree.CheckNode <tree.CheckNode>`
  * :class:`Tree <tree.Tree>`
  * :class:`Tree.CheckTree <tree.CheckTree>`

从已有的html结构生成树
--------------------------------------------------

    .. raw:: html

        <iframe width="100%" height="200" class="iframe-demo" src="../../../_static/demo/tree/demo3.html"></iframe>


    **HTML关键代码**
    
    .. code-block:: html
	
		<div id="treeContainer" style="width: 200px;">
			<!-- 直接通过DOM中已有的结构生成一棵树  -->
			<div id='root' class="ks-tree-root">
				<span class="ks-tree-item-label">淘宝网</span>
				<div class="ks-tree-children">
					<div class="ks-tree-item">
						<span class="ks-tree-item-label">收藏夹</span>
						<div class="ks-tree-children">
							<div class="ks-tree-item">
								<span class="ks-tree-item-label">收藏的宝贝</span>
							</div>
							<div class="ks-tree-item ks-tree-item-folder">
								<span class="ks-tree-item-label">收藏的店铺</span>
							</div>
						</div>
					</div>
					<div class="ks-tree-item">
						<span class="ks-tree-item-label">我要买</span>
					</div>
				</div>
			</div>
		</div>

    **初始化树**

    .. literalinclude:: /_static/demo/tree/assets/demo3.js
           :language: javascript
    
    .. note::

        使用树还需要自己定义皮肤样式, 以上参考的是 `google 的样式 <../../../_static/demo/tree/assets/tree.css>`_
