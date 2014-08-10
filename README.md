graz.at
=======

Original:

```
<ul class="buttons-content left"><li><script type="text/javascript"><!--
$(function() {
    var url = encodeURIComponent($('#social_url').val());
    var title = encodeURIComponent($('#social_title').val()); 
    $('#social_fb_share').attr('href', 'http://www.facebook.com/sharer.php?u=' + url + '&t=' + title);
    $('#social_twitter').attr('href', 'http://twitter.com/home?status=' + title + '%20' + url);
});
--></script><a id="social_fb_share" title="Facebook" target="_blank" style="margin-right:20px"><img src="/2010/g/social-fb-share.gif" alt="socialbuttons" title="Facebook teilen" height="21" width="62" /></a><iframe src="http://www.facebook.com/plugins/like.php?href=http%3A%2F%2Fwww.graz.at/cms/beitrag/10235966/374633&amp;layout=button_count&amp;show_faces=true&amp;width=160&amp;action=like&amp;font=verdana&amp;colorscheme=light&amp;height=21" scrolling="no" frameborder="0" style="border:none; overflow:hidden; width:160px; height:21px;" title="Gefällt mir auf Facebook"><br /></iframe></li>
```


```
<script src="http://leerstand.localhost/socialshareprivacy/jquery-1.11.1.min.js" type="text/javascript"></script>

<script type="text/javascript" src="/SocialSharePrivacy/javascripts/jquery.cookies.js"></script>
<script type="text/javascript" src="/socialshareprivacy/javascripts/socialshareprivacy.js"></script>
<script type="text/javascript" src="/socialshareprivacy/javascripts/modules/fbshare.js"></script>
<script type="text/javascript" src="/socialshareprivacy/javascripts/modules/facebook.js"></script>
<script type="text/javascript" src="/socialshareprivacy/javascripts/locale/de/socialshareprivacy.js"></script>
<script type="text/javascript" src="/socialshareprivacy/javascripts/locale/de/modules/facebook.js"></script>

<script type="text/javascript">
// <![CDATA[
$.fn.socialSharePrivacy.settings.order = ['fbshare', 'facebook'];
$.fn.socialSharePrivacy.settings.path_prefix = '/socialshareprivacy/';
$.fn.socialSharePrivacy.settings.info_link_target = '_blank';
$(document).ready(function () {
	$('.share').socialSharePrivacy();
});
// ]]>
</script>
```
