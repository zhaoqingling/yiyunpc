$(function(){

  var browser=navigator.appName 
  var b_version=navigator.appVersion 
  var version=b_version.split(";"); 
  var trim_Version=version[1].replace(/[ ]/g,"");
  // 切换登录方式
  $(document).on('click', '#change-login', function(){
       $('[login-form]').find('ul').show();
       if(browser=="Microsoft Internet Explorer" && trim_Version=="MSIE8.0") 
        { 
            if($(this).hasClass('phone')){
              $('[login-form]').find('ul').eq(1).hide();
              $('[login-form-wrap]').height('388');
              $(this).removeClass('phone').find('span').text('手机快速登录');
              $(this).find('.icon').html('&#xe613;');
            }else{
              $('[login-form]').find('ul').eq(0).hide();
              $('[login-form-wrap]').height('492');
              $(this).addClass('phone').find('span').text('普通登录');
              $(this).find('.icon').html('&#xe64c;');
            }
        }else{
            // 手机登录或者普通登录
            if($(this).hasClass('phone')){
              $('[login-form]').css({
                'transform':'translateX(0)'
              });
              $('[login-form-wrap]').height('388');
              $(this).removeClass('phone').find('span').text('手机快速登录');
              $(this).find('.icon').html('&#xe613;');
             // $('[login-form]').find('ul').eq(1).hide();
            }else{
              $('[login-form]').css({
                'transform':'translateX(-400px)'
              });
              $('[login-form-wrap]').height('492');
              $(this).addClass('phone').find('span').text('普通登录');
              $(this).find('.icon').html('&#xe64c;');
             // $('[login-form]').find('ul').eq(0).hide();
            }
        } 
    
  });
  //点击显示金山账号弹窗
    $(document).on('click','[other-account]',function(){
        $('[mask]').removeClass('undis');
        $('[account-dialog]').removeClass('undis');
        return false;
    });

  //点击金山账号弹窗关闭按钮
  $(document).on('click','[account-close]',function(){
        $('[mask]').addClass('undis');
        $('[account-dialog]').addClass('undis');
        return false;
  });  

	//banner
	$('#slider').cycleSlider({
		fx:'fade',
		speed:400,
		timeout:4000,
		pause:true,
		pager:'#sliderNum',
		pagerEvent:'mouseover'
	});

});
