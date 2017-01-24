# uploadPreview
①uploadPreview实现图片上传立即显示 ，
②附上 多图上传 ，增加减少dom节点的js操作

#使用步骤：1.引入uploadPreview包
<script type="text/javascript" src="{$Think.config.COMMON_URL}Js/jquery-1.11.3.min.js"></script>
2.，按以下格式写html代码，给input表单添加id ,给外层div添加id，给img添加id
<td><input type='file' name='goods_pics[]' id="goods_pics_0" />
                        <div id="goods_pics_dv_0"><img src="" alt="" width="160" height="160" id="goods_pics_im_0"/></div>
                        </td>
3.js代码中引入2步骤定义的input表单id，div的id，img的id                    
<script type="text/javascript">
                $(function(){
                    new uploadPreview({ UpBtn: "goods_pics_0", DivShow: "goods_pics_dv_0", ImgShow: "goods_pics_im_0" });
                });
                </script>	

