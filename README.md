
<!DOCTYPE html>
<!-- set this class so CSS definitions that now use REM size, would work relative to this.
	Since now almost everything is relative to one of the 2 absolute font size classese -->
<html class="user_font_size_normal" lang="en">
<head>
<!--
 login.jsp
 * ***** BEGIN LICENSE BLOCK *****
 * Zimbra Collaboration Suite Web Client
 * Copyright (C) 2007, 2008, 2009, 2010, 2011, 2012, 2013, 2014, 2015, 2016 Synacor, Inc.
 *
 * This program is free software: you can redistribute it and/or modify it under
 * the terms of the GNU General Public License as published by the Free Software Foundation,
 * version 2 of the License.
 *
 * This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 * without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 * See the GNU General Public License for more details.
 * You should have received a copy of the GNU General Public License along with this program.
 * If not, see <https://www.gnu.org/licenses/>.
 * ***** END LICENSE BLOCK *****
-->
	<meta http-equiv="Content-Type" content="text/html;charset=utf-8">
	<title>Zimbra Web Client Sign In</title>
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<meta name="description" content="Zimbra provides open source server and client software for messaging and collaboration. To find out more visit https://www.zimbra.com.">
	<meta name="apple-mobile-web-app-capable" content="yes" />
	<meta name="apple-mobile-web-app-status-bar-style" content="black" />
	<link rel="stylesheet" type="text/css" href="/css/common,login,zhtml,skin.css?skin=harmony&v=230406110552">
	<link rel="SHORTCUT ICON" href="/img/logo/favicon.ico">


</head>
<body onload="onLoad();">

	<div class="LoginScreen">
		<div class="center">
			<div class="contentBox">
				<h1><a href="https://www.zimbra.com/" id="bannerLink" target="_new" title='Zimbra'><span class="ScreenReaderOnly">Zimbra</span>
					<span class="ImgLoginBanner"></span>
				</a></h1>
				<div id="ZLoginAppName">Web Client</div>
				<form method="post" name="loginForm" action="/" accept-charset="UTF-8">
								<input type="hidden" name="loginOp" value="login"/>
								<input type="hidden" name="login_csrf" value="aa7d1fdd-e34e-47c5-a624-afbaf8951c0e"/>

								<table class="form">
                        <tr>
                                        <td><label for="username">Username:</label></td>
                                        <td><input id="username" class="zLoginField" name="username" type="text" value="" size="40" maxlength="1024" autocapitalize="off" autocorrect="off"/></td>
                                        </tr>
                                        <tr>
                                <td><label for="password">Password:</label></td>
                                <td><input id="password" autocomplete="off" class="zLoginField" name="password" type="password" value="" size="40" maxlength="1024"/></td>
                                </tr>
                                <tr>
                                <td>&nbsp;</td>
                                <td class="submitTD">
                                <input id="remember" value="1" type="checkbox" name="zrememberme" />
                                    <label for="remember">Stay signed in</label>
                                <input type="submit" class="ZLoginButton DwtButton" value="Sign In" />
                                </td>
                                </tr>
			
				<tr>
                            <td colspan="2"><hr/></td>
                            </tr>
                            <tr>
                            <td>
                            <label for="client">Version:</label>
                            </td>
                            <td>
                            <div class="positioning">
                                <select id="client" name="client" onchange="clientChange(this.options[this.selectedIndex].value)">
                                    <option value="preferred" selected > Default</option>
                                    <option value="advanced" > Advanced (Ajax)</option>
                                    <option value="standard" > Standard (HTML)</option>
                                    <option value="mobile" > Mobile</option>
                                    </select>
                                <script TYPE="text/javascript">
                                document.write("<a href='#' onclick='showWhatsThis();' id='ZLoginWhatsThisAnchor' aria-controls='ZLoginWhatsThis' aria-expanded='false'>What’s This?</a>");
                                </script>
                                <div id="ZLoginWhatsThis" class="ZLoginInfoMessage" style="display:none;" onclick='showWhatsThis();' role="tooltip"><h3 style="text-align:center;">Client Types</h3>	<b>Advanced</b> offers the full set of Web collaboration features. This Web Client works best with newer browsers and faster Internet connections. <br><br><b>Standard</b> is recommended when Internet connections are slow, when using older browsers, or for easier accessibility. <br><br><b>Mobile</b> is recommended for mobile devices. <br><br>To set <b>Default</b> to be your preferred client type, change the sign in options in your Preferences, General tab after you sign in.</div>
                                   <div id="ZLoginUnsupported" class="ZLoginInfoMessage" style="display:none;">Note that your web browser or display does not fully support the Advanced version.  We strongly recommend that you use the Standard client.</div>
                            </div>
                            </td>
                            </tr>
                        </table>
                    </form>
			</div>
			<div class="decor1"></div>
		</div>

		<div class="Footer">
			<div id="ZLoginNotice" class="legalNotice-small"><a target="_new" href="https://www.zimbra.com">Zimbra</a> :: the leader in open source messaging and collaboration :: <a target="_new" href="https://blog.zimbra.com">Blog</a> - <a target="_new" href="https://wiki.zimbra.com">Wiki</a> - <a target="_new" href="https://www.zimbra.com/forums">Forums</a></div>
			<div class="copyright">
			Copyright © 2005-2023 Synacor, Inc. All rights reserved. "Zimbra" is a registered trademark of Synacor, Inc.</div>
		</div>
		<div class="decor2"></div>
	</div>
<script>

function ZmSkin(e){
this.hints=this.mergeObjects(ZmSkin.hints,e)
}
ZmSkin.hints={
name:"harmony",version:"1",skin:{
containers:"skin_outer"}
,banner:{
position:"static",url:"http://www.goiania.go.gov.br"}
,userInfo:{
position:"static"}
,search:{
position:"static"}
,quota:{
position:"static"}
,presence:{
width:"40px",height:"24px"}
,appView:{
position:"static"}
,searchResultsToolbar:{
containers:["skin_tr_search_results_toolbar"]}
,newButton:{
containers:["skin_td_new_button"]}
,tree:{
minWidth:"13.5rem",maxWidth:"84rem",containers:["skin_td_tree","skin_td_tree_app_sash"],resizeContainers:["skin_td_tree","skin_container_app_new_button"]}
,topToolbar:{
containers:"skin_spacing_app_top_toolbar"}
,treeFooter:{
containers:"skin_tr_tree_footer"}
,topAd:{
containers:"skin_tr_top_ad"}
,sidebarAd:{
containers:"skin_td_sidebar_ad"}
,bottomAd:{
containers:"skin_tr_bottom_ad"}
,treeTopAd:{
containers:"skin_tr_tree_top_ad"}
,treeBottomAd:{
containers:"skin_tr_tree_bottom_ad"}
,helpButton:{
style:"link",container:"quota",url:""}
,logoutButton:{
style:"link",container:"quota"}
,appChooser:{
position:"static",direction:"LR"}
,toast:{
location:"N",transitions:[{
type:"fade-in",step:5,duration:50}
,{
type:"pause",duration:5000}
,{
type:"fade-out",step:-10,duration:500}
]}
,fullScreen:{
containers:["!skin_td_tree","!skin_td_tree_app_sash"]}
,allAds:{
containers:["skin_tr_top_ad","skin_td_sidebar_ad","skin_tr_bottom_ad","skin_tr_tree_top_ad","skin_tr_tree_bottom_ad"]}
,hideSearchInCompose:true,notificationBanner:"/skins/_base/logos/NotificationBanner_grey.gif?v=230406110552"};
window.BaseSkin=ZmSkin;
ZmSkin.prototype={
show:function(t,e,l){
var a=this.hints[t]&&this.hints[t].containers;
if(a){
if(typeof a=="function"){
a.apply(this,[e!=false]);
skin._reflowApp();
return
}
if(typeof a=="string"){
a=[a]
}
var s=false;
for(var r=0;
r<a.length;
r++){
var h=a[r];
var o=h.replace(/^!/,"");
var n=h!=o;
if(this._showEl(o,n?!e:e)){
s=true
}}
if(s&&!l){
skin._reflowApp()
}}}
,hide:function(e,t){
this.show(e,false,t)
}
,gotoApp:function(e,t){
appCtxt.getAppController().activateApp(e,null,t)
}
,gotoPrefs:function(e){
if(appCtxt.getCurrentAppName()!=ZmApp.PREFERENCES){
var t=new AjxCallback(this,this._gotoPrefPage,[e]);
this.gotoApp(ZmApp.PREFERENCES,t)
}else{
this._gotoPrefPage(e)
}}
,mergeObjects:function(e,o){
if(e==null){
e={}
}
for(var a=1;
a<arguments.length;
a++){
var n=arguments[a];
for(var t in n){
var s=e[t];
if(typeof s=="object"&&!(s instanceof Array)){
this.mergeObjects(e[t],n[t]);
continue
}
if(!e[t]){
e[t]=n[t]
}}}
return e
}
,getTreeWidth:function(){
return Dwt.getSize(this._getEl(this.hints.tree.containers[0])).x
}
,setTreeWidth:function(e){
this._setContainerSizes("tree",e,null)
}
,showTopAd:function(e){
if(skin._showEl("skin_tr_top_ad",e)){
skin._reflowApp()
}}
,hideTopAd:function(){
skin.showTopAd(false)
}
,getTopAdContainer:function(){
return skin._getEl("skin_container_top_ad")
}
,showSidebarAd:function(e){
var t="skin_td_sidebar_ad";
if(e!=null){
Dwt.setSize(t,e)
}
if(skin._showEl(t)){
skin._reflowApp()
}}
,hideSidebarAd:function(){
var e="skin_td_sidebar_ad";
if(skin._hideEl(e)){
skin._reflowApp()
}}
,getSidebarAdContainer:function(){
return this._getEl("skin_container_sidebar_ad")
}
,handleNotification:function(t,e){}
,_getEl:function(e){
return(typeof e=="string"?document.getElementById(e):e)
}
,_showEl:function(o,i){
var t=this._getEl(o);
if(!t){
return
}
var a;
if(i==false){
a="none"
}else{
var e=t.tagName;
if(e=="TD"){
a="table-cell"
}else{
if(e=="TR"){
a="table-row"
}else{
a="block"
}}}
if(a!=t.style.display){
t.style.display=a;
return true
}else{
return false
}}
,_hideEl:function(e){
return this._showEl(e,false)
}
,_reparentEl:function(i,e){
var a=this._getEl(e);
var t=a&&this._getEl(i);
if(t){
a.appendChild(t)
}}
,_setContainerSizes:function(n,a,e){
var o=this.hints[n].resizeContainers||this.hints[n].containers;
for(var t=0;
t<o.length;
t++){
Dwt.setSize(o[t],a,null)
}}
,_reflowApp:function(){
if(window._zimbraMail){
window._zimbraMail.getAppViewMgr().fitAll()
}}
,_gotoPrefPage:function(a){
if(a==null){
return
}
var i=appCtxt.getApp(ZmApp.PREFERENCES);
var t=i.getPrefController();
var e=t.getPrefsView();
e.selectSection(a)
}};
window.skin=new ZmSkin();
var link = document.getElementById("bannerLink");
if (link) {
	link.href = skin.hints.banner.url;
}



// show a message if they should be using the 'standard' client, but have chosen 'advanced' instead
function clientChange(selectValue) {
	var useStandard = false;
	useStandard = useStandard || (screen && (screen.width <= 800 && screen.height <= 600));
	var div = document.getElementById("ZLoginUnsupported");
	if (div)
	div.style.display = ((selectValue == 'advanced') && useStandard) ? 'block' : 'none';
}

// if they have JS, write out a "what's this?" link that shows the message below
function showWhatsThis() {
	var anchor = document.getElementById('ZLoginWhatsThisAnchor'),
        tooltip = document.getElementById("ZLoginWhatsThis"),
        doHide = (tooltip.style.display === "block");
    tooltip.style.display = doHide ? "none" : "block";
    anchor.setAttribute("aria-expanded", doHide ? "false" : "true");
}

function forgotPassword() {
	var accountInput = document.getElementById("username").value;
	var queryParams = encodeURI("account=" + accountInput);
	var url = "/public/PasswordRecovery.jsp?" + location.search;

	if (accountInput !== '') {
		url += (location.search !== '' ? '&' : '') + encodeURI("account=" + accountInput);
	}

	window.location.href = url;
}


function onLoad() {
	var loginForm = document.loginForm;
	if (loginForm.username) {
		if (loginForm.username.value != "") {
			loginForm.password.focus(); //if username set, focus on password
		}
		else {
			loginForm.username.focus();
		}
	}
	clientChange("preferred");
	if (false && loginForm.totpcode) {
        loginForm.totpcode.focus();
	}
}
</script>
</body>
</html>
