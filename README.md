@charset "UTF-8";
* {
  outline: none;
}

body, html {
  margin: 0;
  background: #eee;
  font-family: "Ubuntu", "微軟正黑體", sans-serif;
  letter-spacing: 0.65px;
  font-size: 15px;
  color: #555;
  cursor: default;
}

a {
  text-decoration: none;
  color: #555;
  display: block;
  transition-duration: 0.3s;
}

ul {
  list-style-type: none;
  padding: 0;
}

h3 {
  color: #3d405b;
  margin: 10px 0;
  text-transform: uppercase;
  font-size: 18px;
}

.resume {
  width: 870px;
  background: #fbfbfb;
  margin: 20px auto;
  border: 1px solid #bbb;
  box-shadow: 0 0 20px -3px #bbb;
  position: relative;
  display: flex;
}
.resume::before {
  content: "";
  width: 100%;
  height: 6px;
  background: #8d9e78;
  position: absolute;
  bottom: 0;
  left: 0;
}
.resume::after {
  content: "";
  display: block;
  clear: both;
}
.resume .base, .resume .func {
  box-sizing: border-box;
  float: left;
}
.resume .base > div, .resume .func > div {
  padding-bottom: 10px;
}
.resume .base > div:last-of-type, .resume .func > div:last-of-type {
  padding-bottom: 0;
}
.resume .base {
  width: 225px;
  padding: 30px 15px;
  background: rgba(238, 238, 238, 0.6);
}
.resume .base .profile {
  background: #8d9e78;
  padding: 30px 15px 5px 15px;
  margin: -30px -15px 45px -15px;
  position: relative;
  z-index: 2;
}
.resume .base .profile::after {
  content: "";
  position: absolute;
  background: #8d9e78;
  width: 100%;
  height: 30px;
  bottom: -15px;
  left: 0;
  transform: skewY(-5deg);
  z-index: -1;
}
.resume .base .profile .photo img {
  width: 100%;
  border-radius: 50%;
}
.resume .base .profile .info {
  text-align: center;
  color: #fcfcfc;
}
.resume .base .profile .info .name {
  margin-top: 10px;
  margin-bottom: 0;
  font-size: 1.5em;
  font-weight: normal;
}
.resume .base .contact div {
  line-height: 24px;
}
.resume .base .contact div a:hover {
  color: #e07a5f;
}
.resume .base .contact div a:hover span::after {
  width: 100%;
}
.resume .base .contact div:hover i {
  color: #e07a5f;
}
.resume .base .contact div i {
  color: #8d9e78;
  width: 20px;
  height: 20px;
  font-size: 20px;
  text-align: center;
  margin-right: 15px;
  transition-duration: 0.3s;
}
.resume .base .contact div span {
  position: relative;
}
.resume .base .contact div span::after {
  content: "";
  position: absolute;
  background: #e07a5f;
  height: 1px;
  width: 0;
  bottom: 0;
  left: 0;
  transition-duration: 0.3s;
}
.resume .base .follow .box {
  text-align: center;
  vertical-align: middle;
}
.resume .base .follow .box a {
  display: inline-block;
  vertical-align: text-bottom;
}
.resume .base .follow .box a:hover i {
  background: #e07a5f;
  border-radius: 5px;
  transform: rotate(45deg) scale(0.8);
}
.resume .base .follow .box a:hover i::before {
  transform: rotate(-45deg) scale(1.5);
}
.resume .base .follow .box i {
  display: inline-block;
  font-size: 30px;
  background: #8d9e78;
  width: 60px;
  height: 60px;
  border-radius: 50%;
  line-height: 60px;
  color: #fcfcfc;
  margin: 0 10px 10px 10px;
  transition-duration: 0.3s;
}
.resume .base .follow .box i::before {
  transition-duration: 0.3s;
}
.resume .base .follow .box i.fa::before {
  display: block;
}
.resume .func {
  width: 645px;
  padding: 30px 25px;
}
.resume .func:hover > div {
  transition-duration: 0.3s;
}
.resume .func:hover > div:hover h3 {
  letter-spacing: 1.6px;
}
.resume .func:hover > div:hover h3 i {
  transform: scale(1.2);
}
.resume .func:hover > div:not(:hover) {
  opacity: 0.5;
}
.resume .func h3 {
  transition-duration: 0.3s;
  margin-top: 0;
}
.resume .func h3 i {
  color: #fcfcfc;
  background: #8d9e78;
  width: 42px;
  height: 42px;
  font-size: 20px;
  line-height: 42px;
  border-radius: 50%;
  text-align: center;
  vertical-align: middle;
  margin-right: 8px;
  transition-duration: 0.3s;
}
.resume .func .work, .resume .func .edu {
  float: left;
}
.resume .func .work small, .resume .func .edu small {
  display: block;
  opacity: 0.7;
}
.resume .func .work ul li, .resume .func .edu ul li {
  position: relative;
  margin-left: 15px;
  padding-left: 25px;
  padding-bottom: 15px;
}
.resume .func .work ul li:hover::before, .resume .func .edu ul li:hover::before {
  animation: circle 1.2s infinite;
}
.resume .func .work ul li:hover span, .resume .func .edu ul li:hover span {
  color: #e07a5f;
}
@keyframes circle {
  from {
    box-shadow: 0 0 0 0px #3d405b;
  }
  to {
    box-shadow: 0 0 0 6px rgba(61, 64, 91, 0);
  }
}
.resume .func .work ul li:first-of-type::before, .resume .func .edu ul li:first-of-type::before {
  width: 10px;
  height: 10px;
  left: -2px;
}
.resume .func .work ul li:last-of-type, .resume .func .edu ul li:last-of-type {
  padding-bottom: 3px;
}
.resume .func .work ul li:last-of-type::after, .resume .func .edu ul li:last-of-type::after {
  border-radius: 1.5px;
}
.resume .func .work ul li::before, .resume .func .work ul li::after, .resume .func .edu ul li::before, .resume .func .edu ul li::after {
  content: "";
  display: block;
  position: absolute;
}
.resume .func .work ul li::before, .resume .func .edu ul li::before {
  width: 7px;
  height: 7px;
  border: 3px solid #3d405b;
  background: #fcfcfc;
  border-radius: 50%;
  left: 0;
  z-index: 1;
}
.resume .func .work ul li::after, .resume .func .edu ul li::after {
  width: 3px;
  height: 100%;
  background: #3d405b;
  left: 5px;
  top: 0;
}
.resume .func .work ul li span, .resume .func .edu ul li span {
  transition-duration: 0.3s;
}
.resume .func .work {
  width: 42%;
}
.resume .func .edu {
  width: 58%;
}
.resume .func .skills-prog {
  clear: both;
}
.resume .func .skills-prog ul {
  margin-left: 15px;
}
.resume .func .skills-prog ul li {
  margin-bottom: 8px;
  display: flex;
  align-items: center;
  transition-duration: 0.3s;
}
.resume .func .skills-prog ul li:hover {
  color: #e07a5f;
}
.resume .func .skills-prog ul li:hover .skills-bar .bar {
  background: #e07a5f;
  box-shadow: 0 0 0 1px #e07a5f;
}
.resume .func .skills-prog ul li span {
  display: block;
  width: 120px;
}
.resume .func .skills-prog ul li .skills-bar {
  background: #cdcdcd;
  height: 2px;
  width: calc(100% - 120px);
  position: relative;
  border-radius: 2px;
}
.resume .func .skills-prog ul li .skills-bar .bar {
  position: absolute;
  top: -1px;
  height: 4px;
  background: #8d9e78;
  box-shadow: 0 0 0 #8d9e78;
  border-radius: 5px;
}
.resume .func .skills-soft ul {
  display: flex;
  justify-content: space-between;
  text-align: center;
}
.resume .func .skills-soft ul li {
  position: relative;
}
.resume .func .skills-soft ul li:hover svg .cbar {
  stroke: #e07a5f;
  stroke-width: 4px;
}
.resume .func .skills-soft ul li:hover span, .resume .func .skills-soft ul li:hover small {
  transform: scale(1.2);
}
.resume .func .skills-soft ul li svg {
  width: 95%;
  fill: transparent;
  transform: rotate(-90deg);
}
.resume .func .skills-soft ul li svg circle {
  stroke-width: 1px;
  stroke: #cdcdcd;
}
.resume .func .skills-soft ul li svg .cbar {
  stroke-width: 3px;
  stroke: #8d9e78;
  stroke-linecap: round;
}
.resume .func .skills-soft ul li span, .resume .func .skills-soft ul li small {
  position: absolute;
  display: block;
  width: 100%;
  top: 52%;
  transition-duration: 0.3s;
}
.resume .func .skills-soft ul li span {
  top: 40%;
}
.resume .func .interests-items {
  box-sizing: border-box;
  padding: 15px;
  width: 100%;
  border: 1px solid #cdcdcd;
  text-align: center;
  display: flex;
  justify-content: space-between;
}
.resume .func .interests-items div {
  display: inline-block;
  width: 80px;
  height: 80px;
}
.resume .func .interests-items div:hover i {
  transform: scale(1.2);
}
.resume .func .interests-items div:hover span {
  color: #e07a5f;
  transition-duration: 0.3s;
}
.resume .func .interests-items div i {
  font-size: 45px;
  width: 60px;
  height: 60px;
  line-height: 60px;
  color: #8d9e78;
  transition-duration: 0.3s;
}
.resume .func .interests-items div i.guitar {
  display: block;
  margin: 0 auto;
}
.resume .func .interests-items div i.guitar svg {
  width: 50px;
  height: 50px;
  margin-top: 5px;
  fill: #8d9e78;
}
.resume .func .interests-items div span {
  display: block;
}
(function() {
  $('.skills-prog li').find('.skills-bar').each(function(i) {
    $(this).find('.bar').delay(i * 150).animate({
      width: $(this).parents().attr('data-percent') + '%'
    }, 1000, 'linear', function() {
      return $(this).css({
        'transition-duration': '.5s'
      });
    });
  });

  $('.skills-soft li').find('svg').each(function(i) {
    var c, cbar, circle, percent, r;
    circle = $(this).children('.cbar');
    r = circle.attr('r');
    c = Math.PI * (r * 2);
    percent = $(this).parent().data('percent');
    cbar = ((100 - percent) / 100) * c;
    circle.css({
      'stroke-dashoffset': c,
      'stroke-dasharray': c
    });
    circle.delay(i * 150).animate({
      strokeDashoffset: cbar
    }, 1000, 'linear', function() {
      return circle.css({
        'transition-duration': '.3s'
      });
    });
    $(this).siblings('small').prop('Counter', 0).delay(i * 150).animate({
      Counter: percent
    }, {
      duration: 1000,
      step: function(now) {
        return $(this).text(Math.ceil(now) + '%');
      }
    });
  });

}).call(this);

//# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiPGFub255bW91cz4iXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6IkFBQUE7RUFBQSxDQUFBLENBQUUsaUJBQUYsQ0FBb0IsQ0FBQyxJQUFyQixDQUEwQixhQUExQixDQUF3QyxDQUFDLElBQXpDLENBQThDLFFBQUEsQ0FBQyxDQUFELENBQUE7SUFDNUMsQ0FBQSxDQUFFLElBQUYsQ0FBTyxDQUFDLElBQVIsQ0FBYSxNQUFiLENBQW9CLENBQUMsS0FBckIsQ0FBMkIsQ0FBQSxHQUFFLEdBQTdCLENBQWlDLENBQUMsT0FBbEMsQ0FBMEM7TUFDeEMsS0FBQSxFQUFPLENBQUEsQ0FBRSxJQUFGLENBQU8sQ0FBQyxPQUFSLENBQUEsQ0FBaUIsQ0FBQyxJQUFsQixDQUF1QixjQUF2QixDQUFBLEdBQXlDO0lBRFIsQ0FBMUMsRUFFRyxJQUZILEVBRVMsUUFGVCxFQUVtQixRQUFBLENBQUEsQ0FBQTthQUNqQixDQUFBLENBQUUsSUFBRixDQUFPLENBQUMsR0FBUixDQUFZO1FBQUEscUJBQUEsRUFBdUI7TUFBdkIsQ0FBWjtJQURpQixDQUZuQjtFQUQ0QyxDQUE5Qzs7RUFNQSxDQUFBLENBQUUsaUJBQUYsQ0FBb0IsQ0FBQyxJQUFyQixDQUEwQixLQUExQixDQUFnQyxDQUFDLElBQWpDLENBQXNDLFFBQUEsQ0FBQyxDQUFELENBQUE7QUFDdEMsUUFBQSxDQUFBLEVBQUEsSUFBQSxFQUFBLE1BQUEsRUFBQSxPQUFBLEVBQUE7SUFBRSxNQUFBLEdBQVMsQ0FBQSxDQUFFLElBQUYsQ0FBTyxDQUFDLFFBQVIsQ0FBaUIsT0FBakI7SUFDVCxDQUFBLEdBQUksTUFBTSxDQUFDLElBQVAsQ0FBWSxHQUFaO0lBQ0osQ0FBQSxHQUFJLElBQUksQ0FBQyxFQUFMLEdBQVUsQ0FBQyxDQUFBLEdBQUksQ0FBTDtJQUNkLE9BQUEsR0FBVSxDQUFBLENBQUUsSUFBRixDQUFPLENBQUMsTUFBUixDQUFBLENBQWdCLENBQUMsSUFBakIsQ0FBc0IsU0FBdEI7SUFDVixJQUFBLEdBQU8sQ0FBQyxDQUFDLEdBQUEsR0FBSSxPQUFMLENBQUEsR0FBYyxHQUFmLENBQUEsR0FBc0I7SUFDN0IsTUFBTSxDQUFDLEdBQVAsQ0FBVztNQUFBLG1CQUFBLEVBQXFCLENBQXJCO01BQXdCLGtCQUFBLEVBQW9CO0lBQTVDLENBQVg7SUFDQSxNQUFNLENBQUMsS0FBUCxDQUFhLENBQUEsR0FBRSxHQUFmLENBQW1CLENBQUMsT0FBcEIsQ0FBNEI7TUFDMUIsZ0JBQUEsRUFBa0I7SUFEUSxDQUE1QixFQUVHLElBRkgsRUFFUyxRQUZULEVBRW1CLFFBQUEsQ0FBQSxDQUFBO2FBQ2pCLE1BQU0sQ0FBQyxHQUFQLENBQVc7UUFBQSxxQkFBQSxFQUF1QjtNQUF2QixDQUFYO0lBRGlCLENBRm5CO0lBSUEsQ0FBQSxDQUFFLElBQUYsQ0FBTyxDQUFDLFFBQVIsQ0FBaUIsT0FBakIsQ0FBeUIsQ0FBQyxJQUExQixDQUErQixTQUEvQixFQUEwQyxDQUExQyxDQUE0QyxDQUFDLEtBQTdDLENBQW1ELENBQUEsR0FBRSxHQUFyRCxDQUF5RCxDQUFDLE9BQTFELENBQWtFO01BQ2hFLE9BQUEsRUFBUztJQUR1RCxDQUFsRSxFQUVHO01BQUEsUUFBQSxFQUFVLElBQVY7TUFBZ0IsSUFBQSxFQUFNLFFBQUEsQ0FBQyxHQUFELENBQUE7ZUFDdkIsQ0FBQSxDQUFFLElBQUYsQ0FBTyxDQUFDLElBQVIsQ0FBYSxJQUFJLENBQUMsSUFBTCxDQUFVLEdBQVYsQ0FBQSxHQUFpQixHQUE5QjtNQUR1QjtJQUF0QixDQUZIO0VBWG9DLENBQXRDO0FBTkEiLCJzb3VyY2VzQ29udGVudCI6WyIkKCcuc2tpbGxzLXByb2cgbGknKS5maW5kKCcuc2tpbGxzLWJhcicpLmVhY2ggKGkpIC0+XG4gICQodGhpcykuZmluZCgnLmJhcicpLmRlbGF5KGkqMTUwKS5hbmltYXRlIHtcbiAgICB3aWR0aDogJCh0aGlzKS5wYXJlbnRzKCkuYXR0cignZGF0YS1wZXJjZW50JykgKyAnJSdcbiAgfSwgMTAwMCwgJ2xpbmVhcicsIC0+XG4gICAgJCh0aGlzKS5jc3MgJ3RyYW5zaXRpb24tZHVyYXRpb24nOiAnLjVzJ1xuICByZXR1cm5cbiQoJy5za2lsbHMtc29mdCBsaScpLmZpbmQoJ3N2ZycpLmVhY2ggKGkpIC0+XG4gIGNpcmNsZSA9ICQodGhpcykuY2hpbGRyZW4oJy5jYmFyJylcbiAgciA9IGNpcmNsZS5hdHRyKCdyJylcbiAgYyA9IE1hdGguUEkgKiAociAqIDIpXG4gIHBlcmNlbnQgPSAkKHRoaXMpLnBhcmVudCgpLmRhdGEgJ3BlcmNlbnQnXG4gIGNiYXIgPSAoKDEwMC1wZXJjZW50KS8xMDApICogY1xuICBjaXJjbGUuY3NzICdzdHJva2UtZGFzaG9mZnNldCc6IGMsICdzdHJva2UtZGFzaGFycmF5JzogY1xuICBjaXJjbGUuZGVsYXkoaSoxNTApLmFuaW1hdGUge1xuICAgIHN0cm9rZURhc2hvZmZzZXQ6IGNiYXJcbiAgfSwgMTAwMCwgJ2xpbmVhcicsIC0+XG4gICAgY2lyY2xlLmNzcyAndHJhbnNpdGlvbi1kdXJhdGlvbic6ICcuM3MnXG4gICQodGhpcykuc2libGluZ3MoJ3NtYWxsJykucHJvcCgnQ291bnRlcicsIDApLmRlbGF5KGkqMTUwKS5hbmltYXRlIHtcbiAgICBDb3VudGVyOiBwZXJjZW50XG4gIH0sIGR1cmF0aW9uOiAxMDAwLCBzdGVwOiAobm93KSAtPlxuICAgICQodGhpcykudGV4dCBNYXRoLmNlaWwobm93KSArICclJ1xuICByZXR1cm4iXX0=
//# sourceURL=coffeescript
