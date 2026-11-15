<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<title>Bottle City</title>
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no, viewport-fit=cover">
<style>
:root{--or:#f7a21b;--ink:#f4ead6;--bg:#14100c;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root{--bg:#14100c}}
*{box-sizing:border-box;-webkit-tap-highlight-color:transparent;user-select:none;-webkit-user-select:none}
html,body{margin:0;height:100%;background:var(--bg);overflow:hidden;color:var(--ink);font-family:Georgia,serif}
canvas{display:block;position:fixed;inset:0;width:100%;height:100%;touch-action:none}
.big{font-family:Impact,"Arial Black",sans-serif;letter-spacing:.03em}
.ov{position:fixed;inset:0;display:none}
#lobby{display:flex;flex-wrap:wrap;gap:20px;align-items:center;justify-content:space-between;padding:calc(env(safe-area-inset-top,0px) + 16px) 28px 16px;background:linear-gradient(90deg,rgba(0,0,0,.9),rgba(0,0,0,.25));overflow:auto}
#lobby h1{font-size:clamp(54px,11vw,120px);line-height:.9;margin:0;color:var(--or);-webkit-text-stroke:2px #000;text-shadow:5px 5px 0 #000}
#lobby h2{font-size:18px;margin:6px 0 18px;font-weight:400;opacity:.85}
.pb{font-size:30px;padding:12px 44px;background:var(--or);color:#000;border:3px solid #000;box-shadow:4px 4px 0 #000;cursor:pointer;font-family:Impact,sans-serif}
.pb:focus-visible,.lv:focus-visible,.gc:focus-visible{outline:3px solid #fff;outline-offset:2px}
.pn{background:rgba(10,8,6,.72);border:2px solid #3a2e22;padding:14px;max-width:460px;width:100%}
.pn h3{margin:0 0 10px;font-size:20px;color:var(--or)}
#lv{display:grid;grid-template-columns:repeat(6,1fr);gap:6px}
.lv{font:700 18px Impact,sans-serif;padding:9px 0;background:#2a2118;color:var(--ink);border:2px solid #4a3a28;cursor:pointer}
.lv.sel{background:var(--or);color:#000;border-color:#fff}.lv.lock{opacity:.3;cursor:not-allowed}.lv.done{border-color:#7fd17f}
#gn{display:grid;grid-template-columns:repeat(3,1fr);gap:6px;margin-top:2px}
.gc{background:#2a2118;border:2px solid #4a3a28;color:var(--ink);padding:8px 4px;font:14px Georgia,serif;cursor:pointer;text-align:center}
.gc b{display:block;font:18px Impact,sans-serif;color:var(--or)}.gc.sel{border-color:#fff;background:#4a3320}.gc.lock{opacity:.35}
#hud{position:fixed;left:0;right:0;top:0;padding:calc(env(safe-area-inset-top,0px) + 10px) 16px;display:none;justify-content:space-between;font-size:22px;pointer-events:none;text-shadow:0 2px 6px #000}
#cross{position:fixed;left:50%;top:50%;width:28px;height:28px;margin:-14px;pointer-events:none;display:none}
#cross:before,#cross:after{content:"";position:absolute;background:#fff;box-shadow:0 0 3px #000}
#cross:before{left:13px;top:0;width:2px;height:28px}#cross:after{top:13px;left:0;height:2px;width:28px}
#cross.hit:before,#cross.hit:after{background:#f33}
#rl{position:fixed;left:50%;top:58%;width:200px;margin-left:-100px;text-align:center;display:none;pointer-events:none;font-size:18px}
#rl i{display:block;height:8px;background:#fff3;margin-top:4px}#rl i b{display:block;height:100%;width:0;background:var(--or)}
#flash{position:fixed;inset:0;background:#ffb040;opacity:0;pointer-events:none}
#res,#pause{align-items:center;justify-content:center;flex-direction:column;background:rgba(10,7,4,.85);text-align:center;gap:12px}
#res h1{font-size:clamp(40px,9vw,80px);margin:0;color:var(--or)}#res p{font-size:24px;margin:0}
#res .pb{font-size:22px;padding:8px 26px}
.tb{position:fixed;width:84px;height:84px;border-radius:50%;background:rgba(247,162,27,.3);border:3px solid var(--or);color:#fff;font:15px Impact,sans-serif;display:none;align-items:center;justify-content:center;touch-action:none}
body.touch.playing .tb{display:flex}
#bF{width:108px;height:108px;right:22px;bottom:calc(env(safe-area-inset-bottom,0px) + 28px);font-size:22px}
#bA{right:142px;bottom:calc(env(safe-area-inset-bottom,0px) + 28px)}
#bR{right:22px;bottom:calc(env(safe-area-inset-bottom,0px) + 150px)}
#bG{right:122px;bottom:calc(env(safe-area-inset-bottom,0px) + 130px)}
</style>
</head>
<body>
<div id="hud" class="big"><span id="hL"></span><span id="hT"></span><span id="hK"></span><span id="hA"></span></div>
<div id="cross"></div>
<div id="rl" class="big">RELOADING<i><b id="rb"></b></i></div>
<div id="flash"></div>
<div class="tb" id="bF">FIRE</div><div class="tb" id="bA">AIM</div><div class="tb" id="bR">RELOAD</div><div class="tb" id="bG">GUN</div>
<div id="lobby" class="ov">
  <div><h1 class="big">BOTTLE<br>CITY</h1><h2>Street shooting range. Thirty levels. Six guns.</h2><button class="pb" id="play">PLAY</button></div>
  <div style="display:flex;flex-direction:column;gap:12px;flex:1;min-width:280px;align-items:flex-end">
    <div class="pn"><h3 class="big">Choose level</h3><div id="lv"></div></div>
    <div class="pn"><h3 class="big">Choose gun</h3><div id="gn"></div></div>
  </div>
</div>
<div id="res" class="ov"><h1 class="big" id="rt"></h1><p id="rs"></p><div style="display:flex;gap:10px;flex-wrap:wrap;justify-content:center"><button class="pb" id="rN">NEXT</button><button class="pb" id="rR">RETRY</button><button class="pb" id="rL">LOBBY</button></div></div>
<div id="pause" class="ov"><h1 class="big" style="font-size:52px;margin:0;color:var(--or)">PAUSED</h1><p>Click anywhere to resume</p></div>
<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
<script>
(function(){
const $=i=>document.getElementById(i),touch=matchMedia('(pointer:coarse)').matches||'ontouchstart' in window;
if(touch)document.body.classList.add('touch');
let progress=0;try{progress=+localStorage.getItem('bc_p')||0}catch(e){}
// u = level at which gun unlocks, f = sound filter, spr = aim spread
const G=[
{n:'Pistol',mag:12,rate:.22,rl:1.0,pel:1,spr:0,auto:0,len:.26,c:0x2c2c30,u:1,f:2500,rec:.018},
{n:'Revolver',mag:6,rate:.55,rl:1.7,pel:1,spr:0,auto:0,len:.3,c:0x8a8d94,u:3,f:1600,rec:.05},
{n:'SMG',mag:30,rate:.075,rl:1.4,pel:1,spr:.02,auto:1,len:.34,c:0x1d1d20,u:6,f:3200,rec:.01},
{n:'Shotgun',mag:6,rate:.8,rl:2.1,pel:8,spr:.07,auto:0,len:.62,c:0x3a2a1c,u:10,f:900,rec:.07,stock:1},
{n:'Rifle',mag:30,rate:.1,rl:1.8,pel:1,spr:.008,auto:1,len:.6,c:0x3b4a32,u:15,f:1800,rec:.014,stock:1},
{n:'Sniper',mag:5,rate:1,rl:2.4,pel:1,spr:0,auto:0,len:.8,c:0x20252b,u:20,f:1200,rec:.06,stock:1,scope:1}];
// renderer and scene
const ren=new THREE.WebGLRenderer({antialias:true});
ren.setPixelRatio(Math.min(devicePixelRatio,touch?1.75:2));ren.setSize(innerWidth,innerHeight);
ren.shadowMap.enabled=true;ren.shadowMap.type=THREE.PCFSoftShadowMap;
ren.outputEncoding=THREE.sRGBEncoding;ren.toneMapping=THREE.ACESFilmicToneMapping;ren.toneMappingExposure=1.05;
document.body.prepend(ren.domElement);
const scene=new THREE.Scene(),cam=new THREE.PerspectiveCamera(70,innerWidth/innerHeight,.05,300);
cam.rotation.order='YXZ';cam.position.set(0,1.7,0);scene.add(cam);
function cv(w,h){const c=document.createElement('canvas');c.width=w;c.height=h;return c}
const sc=cv(2,256),sx=sc.getContext('2d'),sg=sx.createLinearGradient(0,0,0,256);
sg.addColorStop(0,'#2b2160');sg.addColorStop(.5,'#d9663a');sg.addColorStop(1,'#ffc27a');sx.fillStyle=sg;sx.fillRect(0,0,2,256);
const sky=new THREE.CanvasTexture(sc);sky.encoding=THREE.sRGBEncoding;scene.background=sky;
scene.fog=new THREE.Fog(0xe39a62,30,120);
scene.add(new THREE.HemisphereLight(0xffc89a,0x3a2a3a,.75));
const sun=new THREE.DirectionalLight(0xffb070,1.5);sun.position.set(-22,26,14);sun.target.position.set(0,0,-22);
sun.castShadow=true;sun.shadow.mapSize.set(touch?1024:2048,touch?1024:2048);
Object.assign(sun.shadow.camera,{left:-32,right:32,top:32,bottom:-32,near:1,far:90});sun.shadow.bias=-.0005;
scene.add(sun,sun.target);
const mf=new THREE.PointLight(0xffc060,0,6);mf.position.set(.2,-.1,-.9);cam.add(mf);
// world
const gnd=new THREE.Mesh(new THREE.PlaneGeometry(300,300),new THREE.MeshStandardMaterial({color:0x2b2b31,roughness:.95}));
gnd.rotation.x=-Math.PI/2;gnd.receiveShadow=true;scene.add(gnd);
const lineM=new THREE.MeshStandardMaterial({color:0xe8e0c0,roughness:.8});
for(let i=0;i<14;i++){const l=new THREE.Mesh(new THREE.BoxGeometry(.18,.02,2),lineM);l.position.set(0,.01,2-i*5);scene.add(l)}
const curb=new THREE.MeshStandardMaterial({color:0x6c675f,roughness:.9});
[-14,14].forEach(x=>{const c=new THREE.Mesh(new THREE.BoxGeometry(6,.25,160),curb);c.position.set(x*1.2,.12,-50);c.receiveShadow=true;scene.add(c)});
function winTex(){const c=cv(64,128),x=c.getContext('2d');x.fillStyle='#15161d';x.fillRect(0,0,64,128);
 for(let r=0;r<16;r++)for(let q=0;q<8;q++){x.fillStyle=Math.random()<.35?(Math.random()<.5?'#ffd27a':'#bfe6ff'):'#262a38';x.fillRect(q*8+1,r*8+1,5,6)}
 const t=new THREE.CanvasTexture(c);t.encoding=THREE.sRGBEncoding;t.wrapS=t.wrapT=THREE.RepeatWrapping;return t}
const wt=[winTex(),winTex(),winTex()];
function tower(x,z,w,h,d,k){const t=wt[k%3].clone();t.needsUpdate=true;t.repeat.set(Math.max(1,w/3),Math.max(1,h/6));
 const m=new THREE.Mesh(new THREE.BoxGeometry(w,h,d),new THREE.MeshStandardMaterial({color:0x8b8070,map:t,emissive:0xffffff,emissiveMap:t,emissiveIntensity:.55,roughness:.85}));
 m.position.set(x,h/2,z);m.castShadow=true;m.receiveShadow=true;scene.add(m)}
for(let i=0;i<16;i++)tower(-62+i*8.2+Math.random()*3,-58-Math.random()*14,6+Math.random()*4,16+Math.random()*28,8,i);
for(let i=0;i<5;i++){tower(-20-Math.random()*4,-8-i*14,9,10+Math.random()*14,10,i);tower(20+Math.random()*4,-8-i*14,9,10+Math.random()*14,10,i+1)}
const crateM=new THREE.MeshStandardMaterial({color:0x7a5230,roughness:.8}),barM=new THREE.MeshStandardMaterial({color:0x9a2f22,roughness:.5,metalness:.4});
[[-4,-5],[4.5,-6.5],[-6.5,-3]].forEach(p=>{const c=new THREE.Mesh(new THREE.BoxGeometry(1,1,1),crateM);c.position.set(p[0],.5,p[1]);c.rotation.y=Math.random();c.castShadow=c.receiveShadow=true;scene.add(c)});
[[3,-3.5],[-8,-6],[8,-4]].forEach(p=>{const b=new THREE.Mesh(new THREE.CylinderGeometry(.4,.4,1,14),barM);b.position.set(p[0],.5,p[1]);b.castShadow=true;scene.add(b)});
// bottles
const prof=[[0,0],[.075,0],[.085,.03],[.085,.27],[.065,.35],[.035,.42],[.032,.5],[.04,.52],[0,.52]].map(p=>new THREE.Vector2(p[0],p[1]));
const bGeo=new THREE.LatheGeometry(prof,14),hGeo=new THREE.BoxGeometry(.3,.65,.3),hMat=new THREE.MeshBasicMaterial({visible:false}),
 capGeo=new THREE.CylinderGeometry(.04,.04,.03,10),capM=new THREE.MeshStandardMaterial({color:0xd8b04a,metalness:.8,roughness:.3}),
 bMats=[0x2fbf70,0x8b5a2b,0x3a9ad8,0xcfd8dc].map(c=>new THREE.MeshStandardMaterial({color:c,transparent:true,opacity:.78,roughness:.08,metalness:.1})),
 woodM=new THREE.MeshStandardMaterial({color:0x6e4524,roughness:.85});
const LG=new THREE.Group();scene.add(LG);let bottles=[],hits=[],left=0,total=1;
function plank(x,y,z,w,h,d){const m=new THREE.Mesh(new THREE.BoxGeometry(w,h,d),woodM);m.position.set(x,y,z);m.castShadow=m.receiveShadow=true;LG.add(m)}
function build(L){
 while(LG.children.length)LG.remove(LG.children[0]);bottles=[];hits=[];
 const N=6+Math.floor(L*.9),R=L<6?2:L<15?3:4,mv=L<4?0:Math.min(.7,(L-3)*.03),sp=.5+L*.05;
 for(let r=0;r<R;r++){
  const z=-10-r*8,y=1+r*.15,n=Math.floor(N/R)+(r<N%R?1:0),span=8+r*4;
  plank(0,y-.06,z,span+3,.12,.7);
  for(let i=0;i<4;i++)plank(-span/2-1+i*(span+2)/3,(y-.12)/2,z,.2,y-.12,.2);
  for(let i=0;i<n;i++){
   const x=-span/2+i*span/(n-1),g=new THREE.Group(),m=new THREE.Mesh(bGeo,bMats[(i+r+L)%4]);
   m.castShadow=true;const cap=new THREE.Mesh(capGeo,capM);cap.position.y=.535;g.add(m,cap);
   const h=new THREE.Mesh(hGeo,hMat);h.position.y=.3;h.userData.b=g;g.add(h);
   g.position.set(x,y,z);g.userData={bx:x,ph:Math.random()*6.3,amp:Math.random()<mv?1.2:0,sp:sp,m:bMats[(i+r+L)%4],d:-z,alive:true};
   LG.add(g);bottles.push(g);hits.push(h)}}
 left=total=bottles.length;
}
// shards
const shards=[],sGeo=new THREE.TetrahedronGeometry(.035);
function shatter(p,mat){for(let i=0;i<20;i++){const s=new THREE.Mesh(sGeo,mat);s.position.copy(p);s.position.y+=.2;
 s.userData={v:new THREE.Vector3((Math.random()-.5)*3,Math.random()*3+.5,(Math.random()-.5)*3+1.5),l:1.3};scene.add(s);shards.push(s)}}
// guns
function buildGun(g){
 const o=new THREE.Group(),m=new THREE.MeshStandardMaterial({color:g.c,metalness:.7,roughness:.35}),w=new THREE.MeshStandardMaterial({color:0x6b4423,roughness:.8});
 const b=(a,h,l,x,y,z,mt)=>{const e=new THREE.Mesh(new THREE.BoxGeometry(a,h,l),mt||m);e.position.set(x,y,z);o.add(e);return e};
 b(.05,.06,g.len,0,0,-g.len/2);
 const br=new THREE.Mesh(new THREE.CylinderGeometry(.013,.013,g.len*.5,10),m);br.rotation.x=Math.PI/2;br.position.set(0,.012,-g.len-g.len*.2);o.add(br);
 b(.045,.13,.06,0,-.09,-.02,w).rotation.x=.3;
 const mag=b(.04,.12,.05,0,-.08,-g.len*.5);
 if(g.stock)b(.04,.07,.24,0,-.01,.15,w);
 if(g.scope){const s=new THREE.Mesh(new THREE.CylinderGeometry(.022,.022,.22,10),m);s.rotation.x=Math.PI/2;s.position.set(0,.065,-g.len*.5);o.add(s)}
 const tip=-g.len*1.4,f=new THREE.Mesh(new THREE.SphereGeometry(.045,8,8),new THREE.MeshBasicMaterial({color:0xffd070}));
 f.position.set(0,.012,tip);f.visible=false;o.add(f);o.userData={mag:mag,fl:f};return o}
// state
let mode='lobby',lvl=Math.min(30,progress+1),gi=0,gun=null,ammo=[],time=0,reloading=false,rlT=0,rs1=0,rs2=0,nextShot=0,recoil=0,kick=0,flT=0,
 yaw=0,pitch=0,ads=0,adsOn=false,firing=false,score=0,hitT=0;
const now=()=>performance.now()/1000;
function setGun(i){if(cam.userData.g)cam.remove(cam.userData.g);gi=i;gun=buildGun(G[i]);cam.add(gun);cam.userData.g=gun;reloading=false;$('rl').style.display='none';hud()}
function usable(i){return progress+1>=G[i].u}
// audio
let ac,nb;function A(){if(!ac){ac=new(window.AudioContext||window.webkitAudioContext)();nb=ac.createBuffer(1,ac.sampleRate*.4,ac.sampleRate);const d=nb.getChannelData(0);for(let i=0;i<d.length;i++)d[i]=(Math.random()*2-1)*Math.pow(1-i/d.length,2.5)}return ac}
function bang(f){try{const c=A(),s=c.createBufferSource(),l=c.createBiquadFilter(),g=c.createGain();s.buffer=nb;l.frequency.value=f;g.gain.value=.55;s.connect(l);l.connect(g);g.connect(c.destination);s.start()}catch(e){}}
function tone(f,d,v){try{const c=A(),o=c.createOscillator(),g=c.createGain();o.type='square';o.frequency.value=f;g.gain.setValueAtTime(v||.06,c.currentTime);g.gain.exponentialRampToValueAtTime(.001,c.currentTime+d);o.connect(g);g.connect(c.destination);o.start();o.stop(c.currentTime+d)}catch(e){}}
// shooting
const ray=new THREE.Raycaster();
function fire(){
 if(mode!=='play'||reloading)return;const g=G[gi],t=now();if(t<nextShot)return;
 if(ammo[gi]<=0){reload();return}
 ammo[gi]--;nextShot=t+g.rate;recoil=1;kick+=g.rec;flT=.05;bang(g.f);
 gun.userData.fl.visible=true;mf.intensity=3;
 const fl=$('flash');fl.style.opacity=.12;setTimeout(()=>fl.style.opacity=0,40);
 for(let p=0;p<g.pel;p++){
  ray.setFromCamera({x:(Math.random()-.5)*2*g.spr*(1-ads*.7),y:(Math.random()-.5)*2*g.spr*(1-ads*.7)},cam);
  const h=ray.intersectObjects(hits,false);
  for(const q of h){const b=q.object.userData.b;if(b.userData.alive){
   b.userData.alive=false;LG.remove(b);hits.splice(hits.indexOf(q.object),1);left--;score+=Math.round(b.userData.d*3);
   shatter(b.position,b.userData.m);tone(2200+Math.random()*900,.25,.05);hitT=.12;break}}
 }
 if(ammo[gi]===0)setTimeout(reload,200);
 if(left<=0)finish(true);
}
function reload(){const g=G[gi];if(reloading||mode!=='play'||ammo[gi]>=g.mag)return;reloading=true;rlT=0;rs1=rs2=0;tone(300,.07);$('rl').style.display='block'}
// UI
function hud(){const g=G[gi];$('hL').textContent='LEVEL '+lvl;$('hT').textContent=Math.ceil(Math.max(0,time))+'s';$('hK').textContent='BOTTLES '+left;
 $('hA').textContent=g.n.toUpperCase()+'  '+(ammo[gi]==null?g.mag:ammo[gi])+'/'+g.mag}
function lobbyUI(){
 $('lv').innerHTML='';for(let i=1;i<=30;i++){const b=document.createElement('button');b.className='lv'+(i===lvl?' sel':'')+(i>progress+1?' lock':'')+(i<=progress?' done':'');b.textContent=i;
  b.onclick=()=>{if(i<=progress+1){lvl=i;lobbyUI()}};$('lv').appendChild(b)}
 $('gn').innerHTML='';G.forEach((g,i)=>{const b=document.createElement('button');b.className='gc'+(i===gi?' sel':'')+(usable(i)?'':' lock');
  b.innerHTML='<b>'+g.n+'</b>'+(usable(i)?'Mag '+g.mag:'Unlock at level '+g.u);b.onclick=()=>{if(usable(i)){setGun(i);lobbyUI()}};$('gn').appendChild(b)})}
function show(id,on){$(id).style.display=on?(id==='lobby'?'flex':id==='res'||id==='pause'?'flex':'block'):'none'}
function playUI(on){document.body.classList.toggle('playing',on);$('hud').style.display=on?'flex':'none';$('cross').style.display=on?'block':'none';if(!on)$('rl').style.display='none'}
function lockPtr(){if(!touch&&ren.domElement.requestPointerLock)ren.domElement.requestPointerLock()}
function toLobby(){mode='lobby';playUI(false);show('res',0);show('pause',0);if(document.exitPointerLock&&document.pointerLockElement)document.exitPointerLock();build(1);lobbyUI();show('lobby',1)}
function start(L){lvl=L;build(L);ammo=G.map(g=>g.mag);time=30+total*1.3;score=0;yaw=pitch=kick=0;ads=0;adsOn=false;if(!usable(gi))setGun(0);else setGun(gi);
 reloading=false;mode='play';show('lobby',0);show('res',0);playUI(true);hud();lockPtr()}
function finish(win){if(mode!=='play')return;mode='done';playUI(false);if(document.exitPointerLock)document.exitPointerLock();
 const pct=time/(30+total*1.3),st=pct>.5?3:pct>.25?2:1;
 if(win&&lvl>progress){progress=lvl;try{localStorage.setItem('bc_p',progress)}catch(e){}}
 $('rt').textContent=win?(lvl===30?'ALL 30 CLEARED':'LEVEL '+lvl+' CLEAR'):'TIME UP';
 $('rs').textContent=win?'\u2605'.repeat(st)+'\u2606'.repeat(3-st)+'   Score '+score:left+' bottles left';
 $('rN').style.display=win&&lvl<30?'inline-block':'none';show('res',1)}
$('play').onclick=()=>{A();start(lvl)};$('rN').onclick=()=>start(lvl+1);$('rR').onclick=()=>start(lvl);$('rL').onclick=toLobby;
$('pause').onclick=()=>{mode='play';show('pause',0);lockPtr()};
// input
const cvs=ren.domElement;
function look(dx,dy,s){const k=s*(cam.fov/70);yaw=Math.max(-1.4,Math.min(1.4,yaw-dx*k));pitch=Math.max(-.7,Math.min(.7,pitch-dy*k))}
addEventListener('mousemove',e=>{if(mode==='play'&&document.pointerLockElement===cvs)look(e.movementX,e.movementY,.0022)});
addEventListener('mousedown',e=>{if(mode!=='play'||document.pointerLockElement!==cvs)return;if(e.button===0){firing=true;fire()}if(e.button===2)adsOn=true});
addEventListener('mouseup',e=>{if(e.button===0)firing=false;if(e.button===2)adsOn=false});
addEventListener('contextmenu',e=>e.preventDefault());
addEventListener('keydown',e=>{if(e.key==='r'||e.key==='R')reload();const n=+e.key;if(n>=1&&n<=6&&usable(n-1)&&mode==='play'&&gi!==n-1)setGun(n-1)});
document.addEventListener('pointerlockchange',()=>{if(mode==='play'&&!document.pointerLockElement&&!touch){mode='pause';firing=false;show('pause',1)}});
let tid=null,tx=0,ty=0;
cvs.addEventListener('touchstart',e=>{if(tid!==null)return;const t=e.changedTouches[0];tid=t.identifier;tx=t.clientX;ty=t.clientY},{passive:true});
cvs.addEventListener('touchmove',e=>{for(const t of e.changedTouches)if(t.identifier===tid&&mode==='play'){look(t.clientX-tx,t.clientY-ty,.0042);tx=t.clientX;ty=t.clientY}},{passive:true});
const tend=e=>{for(const t of e.changedTouches)if(t.identifier===tid)tid=null};cvs.addEventListener('touchend',tend);cvs.addEventListener('touchcancel',tend);
function hold(id,dn,up){const b=$(id);b.addEventListener('pointerdown',e=>{e.preventDefault();dn()});['pointerup','pointercancel','pointerleave'].forEach(k=>b.addEventListener(k,up))}
hold('bF',()=>{firing=true;fire()},()=>firing=false);
$('bA').addEventListener('pointerdown',e=>{e.preventDefault();adsOn=!adsOn});
$('bR').addEventListener('pointerdown',e=>{e.preventDefault();reload()});
$('bG').addEventListener('pointerdown',e=>{e.preventDefault();if(mode!=='play')return;let n=gi;do{n=(n+1)%6}while(!usable(n));setGun(n)});
addEventListener('resize',()=>{cam.aspect=innerWidth/innerHeight;cam.updateProjectionMatrix();ren.setSize(innerWidth,innerHeight)});
// loop
let last=performance.now()/1000;
function loop(){
 requestAnimationFrame(loop);const t=now(),dt=Math.min(t-last,.05);last=t;
 const g=G[gi];
 if(mode==='play'){time-=dt;if(time<=0){time=0;finish(false)}if(firing&&g.auto)fire();hud()}
 if(mode==='lobby'){yaw=Math.sin(t*.22)*.5;pitch=-.02;ads=0}
 // moving bottles
 for(const b of bottles)if(b.userData.alive&&b.userData.amp)b.position.x=b.userData.bx+Math.sin(t*b.userData.sp+b.userData.ph)*b.userData.amp;
 // reload progress
 if(reloading){rlT+=dt;const k=Math.min(1,rlT/g.rl);$('rb').style.width=k*100+'%';
  if(!rs1&&k>.35){rs1=1;tone(450,.06)}if(!rs2&&k>.7){rs2=1;tone(650,.06)}
  if(k>=1){reloading=false;ammo[gi]=g.mag;tone(900,.08);$('rl').style.display='none'}}
 // gun animation
 ads+=((adsOn&&mode==='play'?1:0)-ads)*Math.min(1,dt*12);
 cam.fov=70+((gi===5?22:46)-70)*ads;cam.updateProjectionMatrix();
 recoil=Math.max(0,recoil-dt*9);kick=Math.max(0,kick-dt*.35);
 const bob=Math.sin(t*1.6)*.003;
 gun.position.set(.2*(1-ads),-.2+.07*ads+bob,-.38+recoil*.06);gun.rotation.set(recoil*.12,0,0);
 gun.visible=!(gi===5&&ads>.8);
 if(reloading){const k=Math.min(1,rlT/g.rl),s=Math.sin(Math.PI*k);
  gun.position.y-=s*.2;gun.position.x-=s*.05;gun.rotation.z=s*.7;gun.rotation.x=-s*.35;
  gun.userData.mag.position.y=-.08-(k>.3&&k<.7?Math.sin((k-.3)/.4*Math.PI)*.18:0)}
 if(flT>0){flT-=dt;if(flT<=0)gun.userData.fl.visible=false}mf.intensity=Math.max(0,mf.intensity-dt*60);
 if(hitT>0){hitT-=dt;$('cross').classList.add('hit')}else $('cross').classList.remove('hit');
 cam.rotation.set(pitch+kick,yaw,0);
 for(let i=shards.length-1;i>=0;i--){const s=shards[i],u=s.userData;u.v.y-=9*dt;s.position.addScaledVector(u.v,dt);s.rotation.x+=dt*9;u.l-=dt;
  if(s.position.y<.03){s.position.y=.03;u.v.set(0,0,0)}if(u.l<=0){scene.remove(s);shards.splice(i,1)}}
 ren.render(scene,cam);
}
setGun(0);toLobby();loop();
})();
</script>
</body>
</html>
