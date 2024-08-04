
<style> 
@charset "utf-8";
/* CSS Document */
body			{ background: #def; font-family: 'Century Gothic', 'Lucida Grande', 'Microsoft JhengHei', '微軟正黑體', Tahoma, PMingLiu; font-size: 12px; text-align: center; }

div#main		{ margin: 10px auto; background: #fff; width: 650px; border: 1px solid #ccc; box-shadow: 5px 5px 10px 2px #ccc; }
div#ins			{ position: relative; margin: 4px; height: 480px; overflow: hidden; border: 1px solid #ccc; }
span.red		{ color: #f44; }

div.draw div					{ position: absolute; -webkit-transform-origin: 50% 0%; -ms-transform-origin: 50% 0%; -moz-transform-origin: 50% 0%; -o-transform-origin: 50% 0%; }


div.draw div#bubble				{ opacity: 0; }
div.draw:hover div#bubble		{ opacity: 0.8; }
div.draw div#hand				{ margin: 180px 0 0; }
div.draw:hover div#hand			{ margin: 0; }

/*背景*/
div#bg			{ position: absolute; background: -ms-linear-gradient(top left, #7b52a0 30% , #3A397B 70%); background: -moz-linear-gradient(top left, #7b52a0 30% , #3A397B 70%); background: -o-linear-gradient(top left, #7b52a0 30% , #3A397B 70%); background: -webkit-linear-gradient(top left, #7b52a0 30% , #3A397B 70%); width: 100%; height: 100%; left: 0; top: 0; }

/*髮(後)*/
div#hair_back	{  }
div.hb1			{ width: 20px; height: 30px; top: 220px; left: 525px; background: #6a94e0; }
div.hb2			{ width: 20px; height: 30px; top: 340px; left: 205px; background: #4970ab; }
div.hb3			{ width: 170px; height: 170px; top: 50px; left: 498px; -ms-transform: rotate(39deg) skew(10deg,10deg); -moz-transform: rotate(39deg) skew(10deg,10deg); -o-transform: rotate(39deg) skew(10deg,10deg); -webkit-transform: rotate(39deg) skew(10deg,10deg); background: #6a94e0; border-top: 2px solid #000; border-right: 2px solid #000; border-radius: 0 170px; }
div.hb4			{ width: 100px; height: 150px; top: 234px; left: 468px; -ms-transform: rotate(8deg); -moz-transform: rotate(8deg); -o-transform: rotate(8deg); -webkit-transform: rotate(8deg); background: #6a94e0; border-right: 2px solid #000; }
div.hb5			{ width: 100px; height: 150px; top: 348px; left: 454px; -ms-transform: rotate(2deg); -moz-transform: rotate(2deg); -o-transform: rotate(2deg); -webkit-transform: rotate(2deg); background: #6a94e0; border-radius: 0; }
div.hb6			{ width: 100px; height: 68px; top: 348px; left: 452px; -ms-transform: rotate(2deg); -moz-transform: rotate(2deg); -o-transform: rotate(2deg); -webkit-transform: rotate(2deg); border-right: 2px solid #000; }
div.hb7			{ width: 30px; height: 30px; top: 435px; left: 540px; -ms-transform: rotate(45deg) skew(30deg,30deg); -moz-transform: rotate(45deg) skew(30deg,30deg); -o-transform: rotate(45deg) skew(30deg,30deg); -webkit-transform: rotate(45deg) skew(30deg,30deg); background: #6a94e0; border-top: 4px solid #000; border-right: 4px solid #000; border-radius: 0 30px; }

/*脖子*/
div#neck		{  }
div.neck1		{ width: 130px; height: 120px; left: 280px; top: 370px; background: #d2a38f; }
div.neck2		{ width: 5px; height: 5px; left: 312px; top: 400px; -ms-transform: rotate(33deg) skew(30deg,30deg); -moz-transform: rotate(33deg) skew(30deg,30deg); -o-transform: rotate(33deg) skew(30deg,30deg); -webkit-transform: rotate(33deg) skew(30deg,30deg); border-top: 2px solid #000; border-right: 2px solid #000; border-radius: 0 5px; }

/*衣服*/
div#clothes		{  }
div.clothes1	{ width: 95px; height: 110px; left: 452px; top: 360px; background: #5e71ab; border-radius: 0 90px 0 0 / 0 110px 0 0; }
div.clothes2	{ width: 20px; height: 20px; left: 521px; top: 405px; background: #f8f8f8; -ms-transform: rotate(60deg); -moz-transform: rotate(60deg); -o-transform: rotate(60deg); -webkit-transform: rotate(60deg); }
div.clothes3	{ width: 80px; height: 19px; left: 429px; top: 405px; background: #f8f8f8; -ms-transform: rotate(-40deg) skew(17deg,17deg); -moz-transform: rotate(-40deg) skew(17deg,17deg); -o-transform: rotate(-40deg) skew(17deg,17deg); -webkit-transform: rotate(-40deg) skew(17deg,17deg); border-top: 2px solid #000; border-right: 2px solid #000; border-radius: 0 10px 0 0; }
div.clothes4	{ width: 20px; height: 20px; left: 526px; top: 417px; background: #5e71ab; -ms-transform: rotate(60deg); -moz-transform: rotate(60deg); -o-transform: rotate(60deg); -webkit-transform: rotate(60deg); }
div.clothes5	{ width: 80px; height: 19px; left: 436px; top: 415px; background: #5e71ab; -ms-transform: rotate(-40deg) skew(16deg,15deg); -moz-transform: rotate(-40deg) skew(16deg,15deg); -o-transform: rotate(-40deg) skew(16deg,15deg); -webkit-transform: rotate(-40deg) skew(16deg,15deg); border-top: 2px solid #000; border-right: 2px solid #000; border-radius: 0 10px 0 0; }
div.clothes6	{ width: 15px; height: 15px; left: 533px; top: 423px; background: #f8f8f8; -ms-transform: rotate(64deg); -moz-transform: rotate(64deg); -o-transform: rotate(64deg); -webkit-transform: rotate(64deg); }
div.clothes7	{ width: 90px; height: 19px; left: 430px; top: 425px; background: #f8f8f8; -ms-transform: rotate(-40deg) skew(16deg,16deg); -moz-transform: rotate(-40deg) skew(16deg,16deg); -o-transform: rotate(-40deg) skew(16deg,16deg); -webkit-transform: rotate(-40deg) skew(16deg,16deg); border-top: 2px solid #000; border-right: 2px solid #000; border-radius: 0 10px 0 0; }
div.clothes8	{ width: 100px; height: 25px; left: 423px; top: 437px; background: #5e71ab; -ms-transform: rotate(-38deg) skew(13deg,13deg); -moz-transform: rotate(-38deg) skew(13deg,13deg); -o-transform: rotate(-38deg) skew(13deg,13deg); -webkit-transform: rotate(-38deg) skew(13deg,13deg); border-top: 2px solid #000; border-right: 2px solid #000; border-radius: 0 10px 0 0; }
div.clothes9	{ width: 90px; height: 110px; left: 457px; top: 360px; border-top: 2px solid #000; border-right: 2px solid #000; border-radius: 0 90px 0 0 / 0 110px 0 0; }
div.clothes10	{ width: 110px; height: 50px; left: 421px; top: 457px; background: #f8f8f8; -ms-transform: rotate(-28deg) skew(4deg,4deg); -moz-transform: rotate(-28deg) skew(4deg,4deg); -o-transform: rotate(-28deg) skew(4deg,4deg); -webkit-transform: rotate(-28deg) skew(4deg,4deg); border-top: 2px solid #000; border-right: 2px solid #000; border-radius: 0 20px 0 0; }
div.clothes11	{ width: 70px; height: 70px; left: 280px; top: 450px; background: #f8f8f8; -ms-transform: rotate(32.5deg); -moz-transform: rotate(32.5deg); -o-transform: rotate(32.5deg); -webkit-transform: rotate(32.5deg); border-top: 2px solid #000; overflow: hidden; }
div.clothes11a	{ width: 30px; height: 45px; background: #cbc8dd; -ms-transform: rotate(-53deg) skew(18deg,18deg); -moz-transform: rotate(-53deg) skew(18deg,18deg); -o-transform: rotate(-53deg) skew(18deg,18deg); -webkit-transform: rotate(-53deg) skew(18deg,18deg); margin: -10px 0 0 -6px; border-radius: 0 15px; }
div.clothes12	{ width: 85px; height: 120px; left: 219px; top: 370px; background: #5e71ab; -ms-transform: rotate(20deg); -moz-transform: rotate(20deg); -o-transform: rotate(20deg); -webkit-transform: rotate(20deg); border-right: 2px solid #000; overflow: hidden; }
div.clothes12a	{ width: 45px; height: 42px; background: #495384; -ms-transform: rotate(8deg) skew(30deg,30deg); -moz-transform: rotate(8deg) skew(30deg,30deg); -o-transform: rotate(8deg) skew(30deg,30deg); -webkit-transform: rotate(8deg) skew(30deg,30deg); margin: 0 0 0 36px; border-radius: 0 10px; }
div.clothes12b	{ width: 20px; height: 35px; background: #495384; margin: 0 0 0 67px; }
div.clothes13	{ width: 10px; height: 120px; left: 274px; top: 432px; background: #5e71ab; -ms-transform: rotate(15deg); -moz-transform: rotate(15deg); -o-transform: rotate(15deg); -webkit-transform: rotate(15deg); border-right: 2px solid #000; }
div.clothes14	{ width: 70px; height: 90px; left: 193px; top: 355px; background: #f8f8f8; -ms-transform: rotate(-35deg) skew(-30deg,-30deg); -moz-transform: rotate(-35deg) skew(-30deg,-30deg); -o-transform: rotate(-35deg) skew(-30deg,-30deg); -webkit-transform: rotate(-35deg) skew(-30deg,-30deg); border-top: 2px solid #000; border-left: 2px solid #000; border-radius: 40px 0 / 60px 0; }
div.clothes15	{ width: 60px; height: 80px; left: 205px; top: 365px; background: #5e71ab; -ms-transform: rotate(-35deg) skew(-28deg,-28deg); -moz-transform: rotate(-35deg) skew(-28deg,-28deg); -o-transform: rotate(-35deg) skew(-28deg,-28deg); -webkit-transform: rotate(-35deg) skew(-28deg,-28deg); border-top: 2px solid #000; border-left: 2px solid #000; border-radius: 40px 0 / 70px 0; }
div.clothes16	{ width: 50px; height: 140px; left: 400px; top: 389px; background: #5e71ab; -ms-transform: rotate(35deg); -moz-transform: rotate(35deg); -o-transform: rotate(35deg); -webkit-transform: rotate(35deg); border-left: 2px solid #000; overflow: hidden; }
div.clothes16a	{ width: 70px; height: 90px; -ms-transform: rotate(39deg); -moz-transform: rotate(39deg); -o-transform: rotate(39deg); -webkit-transform: rotate(39deg); background: #495384; margin: 20px 0 0 -8px; }
div.clothes17	{ width: 50px; height: 70px; left: 135px; top: 415px; background: #f8f8f8; border-top: 2px solid #000; border-left: 2px solid #000; border-radius: 30px 0 0 / 60px 0 0; }

/*髮(右鬢角)*/
div#hair_right	{  }
div.hr1			{ width: 20px; height: 150px; top: 350px; left: 200px; -ms-transform: rotate(4deg); -moz-transform: rotate(4deg); -o-transform: rotate(4deg); -webkit-transform: rotate(4deg); background: #4970ab; border-right: 2px solid #000; }
div.hr2			{ width: 30px; height: 40px; left: 175px; top: 440px; background: #6a94e0; border-radius: 0 30px 0 0; }
div.hr3			{ width: 30px; height: 40px; left: 165px; top: 420px; -ms-transform: rotate(-10deg); -moz-transform: rotate(-10deg); -o-transform: rotate(-10deg); -webkit-transform: rotate(-10deg); background: #6a94e0; }
div.hr4			{ width: 110px; height: 110px; left: 120px; top: 295px; -ms-transform: rotate(41deg) skew(35deg,35deg); -moz-transform: rotate(41deg) skew(35deg,35deg); -o-transform: rotate(41deg) skew(35deg,35deg); -webkit-transform: rotate(41deg) skew(35deg,35deg); background: -ms-linear-gradient(top left, #4970ab 30% , #6a94e0 30%); background: -moz-linear-gradient(top left, #4970ab 30% , #6a94e0 30%); background: -o-linear-gradient(top left, #4970ab 30% , #6a94e0 30%); background: -webkit-linear-gradient(top left, #4970ab 30% , #6a94e0 30%); border-left: 4px solid #000; border-bottom: 4px solid #000; border-radius: 5px 70px; }
div.hr5			{ width: 40px; height: 122px; left: 154px; top: 300px; -ms-transform: rotate(-15deg); -moz-transform: rotate(-15deg); -o-transform: rotate(-15deg); -webkit-transform: rotate(-15deg); background: #4970ab; border-radius: 0 0 32px; }
div.hr6			{ width: 20px; height: 150px; top: 345px; left: 207px; -ms-transform: rotate(-1deg); -moz-transform: rotate(-1deg); -o-transform: rotate(-1deg); -webkit-transform: rotate(-1deg); border-left: 2px solid #000; }
div.hr7			{ width: 80px; height: 80px; left: 135px; top: 346px; -ms-transform: rotate(28deg) skew(35deg,35deg); -moz-transform: rotate(28deg) skew(35deg,35deg); -o-transform: rotate(28deg) skew(35deg,35deg); -webkit-transform: rotate(28deg) skew(35deg,35deg); background: #4970ab; border-radius: 0 80px; }

/*臉部*/
div#face		{  }
div.face1		{ width: 260px; height: 230px; left: 178px; top: 80px; background: #f2d6be; }
div.face2		{ width: 200px; height: 50px; left: 230px; top: 310px; background: #f2d6be; }
div.face3		{ width: 165px; height: 60px; left: 278px; top: 322px; -ms-transform: rotate(-12deg); -moz-transform: rotate(-12deg); -o-transform: rotate(-12deg); -webkit-transform: rotate(-12deg); background: #f2d6be; }
div.face4		{ width: 130px; height: 50px; left: 170px; top: 312px; -ms-transform: rotate(15deg) skew(15deg,15deg); -moz-transform: rotate(15deg) skew(15deg,15deg); -o-transform: rotate(15deg) skew(15deg,15deg); -webkit-transform: rotate(15deg) skew(15deg,15deg); background: #f2d6be; border-left: 1px solid #000; border-bottom: 1px solid #000; border-radius: 0 25px / 0 20px; }
div.face5		{ width: 49px; height: 49px; left: 353px; top: 373px; -ms-transform: rotate(33deg) skew(-33deg,-33deg); -moz-transform: rotate(33deg) skew(-33deg,-33deg); -o-transform: rotate(33deg) skew(-33deg,-33deg); -webkit-transform: rotate(33deg) skew(-33deg,-33deg); background: #f2d6be; border-right: 3px solid #000; border-bottom: 3px solid #000; border-radius: 40px 0; }
div.face6		{ width: 130px; height: 130px; left: 157px; top: 76px; -ms-transform: rotate(-29deg) skew(-30deg,-30deg); -moz-transform: rotate(-29deg) skew(-30deg,-30deg); -o-transform: rotate(-29deg) skew(-30deg,-30deg); -webkit-transform: rotate(-29deg) skew(-30deg,-30deg); background: #d2a38f; border-radius: 70px 0; }
div.face7		{ width: 110px; height: 110px; left: 177px; top: 119px; -ms-transform: rotate(-24deg) skew(-30deg,-30deg); -moz-transform: rotate(-24deg) skew(-30deg,-30deg); -o-transform: rotate(-24deg) skew(-30deg,-30deg); -webkit-transform: rotate(-24deg) skew(-30deg,-30deg); background: #f2d6be; border-radius: 80px 0; }
div.face8		{ width: 60px; height: 60px; left: 250px; top: 165px; -ms-transform: rotate(36deg) skew(35deg,35deg); -moz-transform: rotate(36deg) skew(35deg,35deg); -o-transform: rotate(36deg) skew(35deg,35deg); -webkit-transform: rotate(36deg) skew(35deg,35deg); background: #d2a38f; border-radius: 0 0; }
div.face9		{ width: 40px; height: 40px; left: 276px; top: 205px; -ms-transform: rotate(45deg) skew(35deg,35deg); -moz-transform: rotate(45deg) skew(35deg,35deg); -o-transform: rotate(45deg) skew(35deg,35deg); -webkit-transform: rotate(45deg) skew(35deg,35deg); background: #f2d6be; border-radius: 0 20px; }
div.face10		{ width: 20px; height: 170px; left: 375px; top: 140px; -ms-transform: rotate(-20deg); -moz-transform: rotate(-20deg); -o-transform: rotate(-20deg); -webkit-transform: rotate(-20deg); background: #d2a38f; border-radius: 0; }
div.face11		{ width: 15px; height: 60px; left: 395px; top: 200px; -ms-transform: rotate(9deg); -moz-transform: rotate(9deg); -o-transform: rotate(9deg); -moz-transform: rotate(9deg); background: #d2a38f; border-radius: 0; }
div.face12		{ width: 20px; height: 20px; left: 378px; top: 345px; background: #f7c4b3; border-radius: 15px; box-shadow: 0 0 10px 7px #f7c4b3; }
div.face13		{ width: 20px; height: 20px; left: 192px; top: 305px; background: #f7c4b3; border-radius: 15px; box-shadow: 0 0 10px 7px #f7c4b3; }
div.face14		{ width: 5px; height: 5px; left: 396px; top: 350px; background: #fee9e0; border-radius: 3px; }
div.face15		{ width: 5px; height: 5px; left: 192px; top: 300px; background: #fee9e0; border-radius: 3px; }
div.face16		{ width: 2px; height: 2px; left: 261px; top: 329px; background: #000; border-radius: 1px; }
div.face17		{ width: 5px; height: 5px; left: 393px; top: 338px; background: #000; border-radius: 3px; }
div.face18		{ width: 30px; height: 50px; left: 270px; top: 140px; background: #d2a38f; }

/*耳朵*/
div#ear			{  }
div.ear1		{ width: 40px; height: 40px; top: 300px; left: 440px; -ms-transform: rotate(-24deg); -moz-transform: rotate(-24deg); -o-transform: rotate(-24deg); -webkit-transform: rotate(-24deg); background: #d2a38f; border-bottom: 2px solid #000; }
div.ear2		{ width: 40px; height: 46px; top: 270px; left: 470px;  border: 2px solid #000; background: #f2d6be; border-radius: 23px; }

/*髮(左鬢角)*/
div#hair_left	{  }
div.hl1			{ width: 45px; height: 200px; top: 290px; left: 433px; -ms-transform: rotate(12deg); -moz-transform: rotate(12deg); -o-transform: rotate(12deg); -webkit-transform: rotate(12deg); background: -ms-linear-gradient(top, #4970ab 33% , #6a94e0 33%); background: -moz-linear-gradient(top, #4970ab 33% , #6a94e0 33%); background: -o-linear-gradient(top, #4970ab 33% , #6a94e0 33%); background: -webkit-linear-gradient(top, #4970ab 33% , #6a94e0 33%); border-right: 2px solid #000; }
div.hl2			{ width: 50px; height: 70px; top: 430px; left: 395px; -ms-transform: rotate(27deg); -moz-transform: rotate(27deg); -o-transform: rotate(27deg); -webkit-transform: rotate(27deg); background: #6a94e0; }
div.hl3			{ width: 20px; height: 70px; top: 440px; left: 377px; -ms-transform: rotate(27deg); -moz-transform: rotate(27deg); -o-transform: rotate(27deg); -webkit-transform: rotate(27deg); background: #6a94e0; }
div.hl4			{ width: 60px; height: 60px; top: 377px; left: 408px; -ms-transform: rotate(-2deg) skew(-37deg,-37deg); -moz-transform: rotate(-2deg) skew(-37deg,-37deg); -o-transform: rotate(-2deg) skew(-37deg,-37deg); -webkit-transform: rotate(-2deg) skew(-37deg,-37deg); background: #4970ab; border-radius: 55px 0; }
div.hl5			{ width: 20px; height: 20px; top: 430px; left: 374px; -ms-transform: rotate(-10deg) skew(-30deg,-30deg); -moz-transform: rotate(-10deg) skew(-30deg,-30deg); -o-transform: rotate(-10deg) skew(-30deg,-30deg); -webkit-transform: rotate(-10deg) skew(-30deg,-30deg); background: #4970ab; border-radius: 20px 0; }
div.hl6			{ width: 20px; height: 70px; top: 440px; left: 377px; -ms-transform: rotate(27deg); -moz-transform: rotate(27deg); -o-transform: rotate(27deg); -webkit-transform: rotate(27deg); border-left: 2px solid #000; }
div.hl7			{ width: 32px; height: 25px; top: 376px; left: 405px; -ms-transform: rotate(19deg); -moz-transform: rotate(19deg); -o-transform: rotate(19deg); -webkit-transform: rotate(19deg); background: #4970ab; border-radius: 0 0 10px; }
div.hl8			{ width: 25px; height: 25px; top: 348px; left: 424px; -ms-transform: rotate(-42deg); -moz-transform: rotate(-42deg); -o-transform: rotate(-42deg); -webkit-transform: rotate(-42deg); background: #4970ab; }
div.hl9			{ width: 35px; height: 100px; top: 283px; left: 434px; -ms-transform: rotate(17deg); -moz-transform: rotate(17deg); -o-transform: rotate(17deg); -webkit-transform: rotate(17deg); background: #4970ab; border-left: 2px solid #000; }
div.hl10		{ width: 20px; height: 70px; top: 377px; left: 405px; -ms-transform: rotate(24deg); -moz-transform: rotate(24deg); -o-transform: rotate(24deg); -webkit-transform: rotate(24deg); background: #4970ab; border-left: 2px solid #000; border-radius: 0 0 20px / 0 0 30px; }
div.hl11		{ width: 53px; height: 53px; top: 315px; left: 395px; -ms-transform: rotate(-23deg) skew(-35deg,-35deg); -moz-transform: rotate(-23deg) skew(-35deg,-35deg); -o-transform: rotate(-23deg) skew(-35deg,-35deg); -webkit-transform: rotate(-23deg) skew(-35deg,-35deg); border-right: 4px solid #000; border-bottom: 4px solid #000; border-radius: 53px 0; }

/*髮(前)*/
div#hair_front	{  }
div.hair_front	{  }
div.hf1			{ width: 20px; height: 80px; top: 150px; left: 400px; -ms-transform: rotate(-20deg); -moz-transform: rotate(-20deg); -o-transform: rotate(-20deg); -webkit-transform: rotate(-20deg); background: #6a94e0; }
div.hf2			{ width: 175px; height: 180px; top: -20px; left: 360px; background: #6a94e0; }

div#hair_frontl1	{  }
div.hfl1a			{ width: 40px; height: 15px; top: 0; left: 73px; background: #6a94e0; }
div.hfl1b			{ width: 100px; height: 15px; top: 18px; left: 25px; -ms-transform: rotate(-30deg); -moz-transform: rotate(-30deg); -o-transform: rotate(-30deg); -webkit-transform: rotate(-30deg); background: #6a94e0; }
div.hfl1c			{ width: 100px; height: 15px; top: 1px; left: 60px; -ms-transform: rotate(-12deg); -moz-transform: rotate(-12deg); -o-transform: rotate(-12deg); -webkit-transform: rotate(-12deg); background: #6a94e0; }
div.hfl1d			{ width: 55px; height: 55px; top: 9px; left: 30px; -ms-transform: rotate(-5deg) skew(-31deg,-31deg); -moz-transform: rotate(-5deg) skew(-31deg,-31deg); -o-transform: rotate(-5deg) skew(-31deg,-31deg); -webkit-transform: rotate(-5deg) skew(-31deg,-31deg); background: #6a94e0; border-top: 3px solid #000; border-left: 3px solid #000; border-radius: 55px 0; }
div.hfl1e			{ width: 63px; height: 63px; top: 23px; left: 57px; -ms-transform: rotate(12deg) skew(-31deg,-31deg); -moz-transform: rotate(12deg) skew(-31deg,-31deg); -o-transform: rotate(12deg) skew(-31deg,-31deg); -webkit-transform: rotate(12deg) skew(-31deg,-31deg); border-top: 3px solid #000; border-left: 3px solid #000; border-radius: 55px 0; }

div#hair_frontl2	{  }
div.hfl2a			{ width: 90px; height: 90px; top: -10px; left: 125px; background: #6a94e0; }
div.hfl2b			{ width: 100px; height: 182px; top: 45px; left: 33px; -ms-transform: rotate(-20deg) skew(-20deg,-20deg); -moz-transform: rotate(-20deg) skew(-20deg,-20deg); -o-transform: rotate(-20deg) skew(-20deg,-20deg); -webkit-transform: rotate(-20deg) skew(-20deg,-20deg); background: #6a94e0; border-top: 2px solid #000; border-left: 2px solid #000; border-radius: 95px 0 / 120px 0; }
div.hfl2c			{ width: 115px; height: 115px; top: 92px; left: 53px; -ms-transform: rotate(-19deg) skew(-29deg,-29deg); -moz-transform: rotate(-19deg) skew(-29deg,-29deg); -o-transform: rotate(-19deg) skew(-29deg,-29deg); -webkit-transform: rotate(-19deg) skew(-29deg,-29deg); background: #4970ab; border-radius: 95px 0 / 100px 0; }
div.hfl2d			{ width: 20px; height: 100px; top: 180px; left: 97px; -ms-transform: rotate(30deg); -moz-transform: rotate(30deg); -o-transform: rotate(30deg); -webkit-transform: rotate(30deg); background: #7b52a0; }
div.hfl2e			{ width: 60px; height: 60px; top: 180px; left: 53px; -ms-transform: rotate(-17deg) skew(-32deg,-32deg); -moz-transform: rotate(-17deg) skew(-32deg,-32deg); -o-transform: rotate(-17deg) skew(-32deg,-32deg); -webkit-transform: rotate(-17deg) skew(-32deg,-32deg); background: #7b52a0; border-top: 4px solid #000; border-left: 4px solid #000; border-radius: 55px 0; }

div#hair_frontl3	{  }
div.hfl3a			{ width: 20px; height: 60px; top: 170px; left: 165px; background: #4970ab; }
div.hfl3b			{ width: 70px; height: 90px; top: 40px; left: 148px; background: #6a94e0; }
div.hfl3c			{ width: 175px; height: 205px; top: 123px; left: 4px; -ms-transform: rotate(-40deg) skew(-12deg,-12deg); -moz-transform: rotate(-40deg) skew(-12deg,-12deg); -o-transform: rotate(-40deg) skew(-12deg,-12deg); -webkit-transform: rotate(-40deg) skew(-12deg,-12deg); background: -ms-linear-gradient(top left, #6a94e0 57% , rgba(106, 148, 224, 0) 57%); background: -moz-linear-gradient(top left, #6a94e0 57% , rgba(106, 148, 224, 0) 57%); background: -o-linear-gradient(top left, #6a94e0 57% , rgba(106, 148, 224, 0) 57%); background: -webkit-linear-gradient(top left, #6a94e0 57% , rgba(106, 148, 224, 0) 57%); border-top: 2px solid #000; border-left: 2px solid #000; border-top-left-radius: 175px; }
div.hfl3d			{ width: 20px; height: 50px; top: 217px; left: 154px; -ms-transform: rotate(22deg); -moz-transform: rotate(22deg); -o-transform: rotate(22deg); -webkit-transform: rotate(22deg); background: #4970ab; }
div.hfl3e			{ width: 135px; height: 135px; top: 143px; left: 95px; -ms-transform: rotate(-33deg) skew(-29deg,-29deg); -moz-transform: rotate(-33deg) skew(-29deg,-29deg); -o-transform: rotate(-33deg) skew(-29deg,-29deg); -webkit-transform: rotate(-33deg) skew(-29deg,-29deg); background: -ms-linear-gradient(top left, #4970ab 47% , rgba(106, 148, 224, 0) 47%); background: -moz-linear-gradient(top left, #4970ab 47% , rgba(106, 148, 224, 0) 47%); background: -o-linear-gradient(top left, #4970ab 47% , rgba(106, 148, 224, 0) 47%); background: -webkit-linear-gradient(top left, #4970ab 47% , rgba(106, 148, 224, 0) 47%); border-radius: 100px 0; }
div.hfl3f			{ width: 65px; height: 65px; top: 264px; left: 120px; -ms-transform: rotate(-32deg) skew(-33deg,-33deg); -moz-transform: rotate(-32deg) skew(-33deg,-33deg); -o-transform: rotate(-32deg) skew(-33deg,-33deg); -webkit-transform: rotate(-32deg) skew(-33deg,-33deg); border-top: 4px solid #000; border-left: 4px solid #000; border-radius: 65px 0; }

div#hair_frontl4	{  }
div.hfl4a			{ width: 130px; height: 70px; top: -10px; left: 148px; background: #6a94e0; }
div.hfl4b			{ width: 60px; height: 45px; top: 10px; left: 215px; background: #6a94e0; }
div.hfl4c			{ width: 35px; height: 100px; top: 45px; left: 227px; -ms-transform: rotate(30deg); -moz-transform: rotate(30deg); -o-transform: rotate(30deg); -webkit-transform: rotate(30deg); background: #6a94e0; }
div.hfl4d			{ width: 15px; height: 15px; top: 276px; left: 168px; -ms-transform: rotate(40deg) skew(35deg,35deg); -moz-transform: rotate(40deg) skew(35deg,35deg); -o-transform: rotate(40deg) skew(35deg,35deg); -webkit-transform: rotate(40deg) skew(35deg,35deg); background: #6a94e0; }
div.hfl4e			{ width: 165px; height: 165px; top: 86px; left: 93px; -ms-transform: rotate(-34deg) skew(-14deg,-15deg); -moz-transform: rotate(-34deg) skew(-14deg,-15deg); -o-transform: rotate(-34deg) skew(-14deg,-15deg); -webkit-transform: rotate(-34deg) skew(-14deg,-15deg); background: -ms-linear-gradient(top left, #6a94e0 45% , rgba(106, 148, 224, 0) 45%); background: -moz-linear-gradient(top left, #6a94e0 45% , rgba(106, 148, 224, 0) 45%); background: -o-linear-gradient(top left, #6a94e0 45% , rgba(106, 148, 224, 0) 45%); background: -webkit-linear-gradient(top left, #6a94e0 45% , rgba(106, 148, 224, 0) 45%); border-top: 2px solid #000; border-left: 2px solid #000; border-radius: 165px 0 }
div.hfl4f			{ width: 155px; height: 155px; top: 87px; left: 151px; -ms-transform: rotate(-23deg) skew(-20deg,-20deg); -moz-transform: rotate(-23deg) skew(-20deg,-20deg); -o-transform: rotate(-23deg) skew(-20deg,-20deg); -webkit-transform: rotate(-23deg) skew(-20deg,-20deg); border-top: 2px solid #000; border-left: 2px solid #000; box-shadow: 2px -27px #4970ab; border-top-left-radius: 165px; }

div#hair_frontl5	{  }
div.hfl5a			{ width: 130px; height: 110px; top: -10px; left: 280px; background: #6a94e0; }
div.hfl5b			{ width: 150px; height: 150px; top: 40px; left: 177px; -ms-transform: rotate(-43deg) skew(-22deg,-22deg); -moz-transform: rotate(-43deg) skew(-22deg,-22deg); -o-transform: rotate(-43deg) skew(-22deg,-22deg); -webkit-transform: rotate(-43deg) skew(-22deg,-22deg); background: -ms-linear-gradient(top left, #6a94e0 48% , rgba(106, 148, 224, 0) 48%); background: -moz-linear-gradient(top left, #6a94e0 48% , rgba(106, 148, 224, 0) 48%); background: -o-linear-gradient(top left, #6a94e0 48% , rgba(106, 148, 224, 0) 48%); background: -webkit-linear-gradient(top left, #6a94e0 48% , rgba(106, 148, 224, 0) 48%); border-top: 2px solid #000; border-left: 2px solid #000; border-radius: 150px 0 }
div.hfl5c			{ width: 30px; height: 170px; top: 92px; left: 252px; overflow: hidden; -ms-transform: rotate(2deg); -moz-transform: rotate(2deg); -o-transform: rotate(2deg); -webkit-transform: rotate(2deg); border-right: 2px solid #000; }
div.hfl5c1			{ width: 80px; height: 80px; margin: 44px 0 0 3px; -ms-transform: rotate(42deg) skew(30deg,30deg); -moz-transform: rotate(42deg) skew(30deg,30deg); -o-transform: rotate(42deg) skew(30deg,30deg); -webkit-transform: rotate(42deg) skew(30deg,30deg); background: #4970ab; border-radius: 0 70px; }

div#hair_frontl6	{  }
div.hfl6a			{ width: 120px; height: 120px; top: 121px; left: 254px; -ms-transform: rotate(34deg) skew(26deg,26deg); -moz-transform: rotate(34deg) skew(26deg,26deg); -o-transform: rotate(34deg) skew(26deg,26deg); -webkit-transform: rotate(34deg) skew(26deg,26deg); background: #6a94e0; border-radius: 0 120px; }
div.hfl6b			{ width: 45px; height: 140px; top: 60px; left: 296px; -ms-transform: rotate(3deg); -moz-transform: rotate(3deg); -o-transform: rotate(3deg); -webkit-transform: rotate(3deg); background: #6a94e0; }
div.hfl6c			{ width: 30px; height: 255px; top: 60px; left: 311px; overflow: hidden; -ms-transform: rotate(3deg); -moz-transform: rotate(3deg); -o-transform: rotate(3deg); -webkit-transform: rotate(3deg); border-right: 2px solid #000; }
div.hfl6c1			{ width: 120px; height: 120px; margin: 65px 0 0 -18px; -ms-transform: rotate(43deg) skew(37deg,37deg); -moz-transform: rotate(43deg) skew(37deg,37deg); -o-transform: rotate(43deg) skew(37deg,37deg); -webkit-transform: rotate(43deg) skew(37deg,37deg); background: #4970ab; border-radius: 0 70px; }
div.hfl6d			{ width: 120px; height: 120px; top: 122px; left: 253px; -ms-transform: rotate(34deg) skew(26deg,26deg); -moz-transform: rotate(34deg) skew(26deg,26deg); -o-transform: rotate(34deg) skew(26deg,26deg); -webkit-transform: rotate(34deg) skew(26deg,26deg); border-left: 2px solid #000; border-bottom: 2px solid #000; border-radius: 0 120px; }

div#hair_frontr1	{  }
div.hfr1a			{ width: 25px; height: 130px; top: 120px; left: 458px; -ms-transform: rotate(-15deg); -moz-transform: rotate(-15deg); -o-transform: rotate(-15deg); -webkit-transform: rotate(-15deg); background: #4970ab; }
div.hfr1b			{ width: 110px; height: 110px; top: 70px; left: 410px; -ms-transform: rotate(15deg) skew(31deg,31deg); -moz-transform: rotate(15deg) skew(31deg,31deg); -o-transform: rotate(15deg) skew(31deg,31deg); -webkit-transform: rotate(15deg) skew(31deg,31deg); background: -ms-linear-gradient(top left, #4970ab 55% , rgba(106, 148, 224, 0) 55%); background: -moz-linear-gradient(top left, #4970ab 55% , rgba(106, 148, 224, 0) 55%); background: -o-linear-gradient(top left, #4970ab 55% , rgba(106, 148, 224, 0) 55%); background: -webkit-linear-gradient(top left, #4970ab 55% , rgba(106, 148, 224, 0) 55%); border-radius: 0 110px; }
div.hfr1c			{ width: 110px; height: 110px; top: 149px; left: 454px; -ms-transform: rotate(28deg) skew(31deg,31deg); -moz-transform: rotate(28deg) skew(31deg,31deg); -o-transform: rotate(28deg) skew(31deg,31deg); -webkit-transform: rotate(28deg) skew(31deg,31deg); background: #4970ab; border-top: 3px solid #000; border-right: 3px solid #000; border-radius: 0 110px; }
div.hfr1d			{ width: 70px; height: 70px; top: 223px; left: 463px; -ms-transform: rotate(16deg) skew(32deg,32deg); -moz-transform: rotate(16deg) skew(32deg,32deg); -o-transform: rotate(16deg) skew(32deg,32deg); -webkit-transform: rotate(16deg) skew(32deg,32deg); background: -ms-linear-gradient(top right, #6a94e0 60% , rgba(106, 148, 224, 0) 60%); background: -moz-linear-gradient(top right, #6a94e0 60% , rgba(106, 148, 224, 0) 60%); background: -o-linear-gradient(top right, #6a94e0 60% , rgba(106, 148, 224, 0) 60%); background: -webkit-linear-gradient(top right, #6a94e0 60% , rgba(106, 148, 224, 0) 60%); border-top: 3px solid #000; border-right: 3px solid #000; border-top-right-radius: 110px; }

div#hair_frontr2	{  }
div.hfr2a			{ width: 150px; height: 150px; top: 157px; left: 408px; -ms-transform: rotate(34deg) skew(27deg,28deg); -moz-transform: rotate(34deg) skew(27deg,28deg); -o-transform: rotate(34deg) skew(27deg,28deg); -webkit-transform: rotate(34deg) skew(27deg,28deg); background: -ms-linear-gradient(top right, #6a94e0 52% , rgba(106, 148, 224, 0) 52%); background: -moz-linear-gradient(top right, #6a94e0 52% , rgba(106, 148, 224, 0) 52%); background: -o-linear-gradient(top right, #6a94e0 52% , rgba(106, 148, 224, 0) 52%); background: -webkit-linear-gradient(top right, #6a94e0 52% , rgba(106, 148, 224, 0) 52%); border-top: 3px solid #000; border-right: 3px solid #000; border-radius: 0 150px; }
div.hfr2b			{ width: 15px; height: 190px; top: 200px; left: 426px; -ms-transform: rotate(-21deg); -moz-transform: rotate(-21deg); -o-transform: rotate(-21deg); -webkit-transform: rotate(-21deg); background: #6a94e0; border-radius: 0 0 15px; }
div.hfr2c			{ width: 30px; height: 180px; top: 150px; left: 410px; -ms-transform: rotate(-21deg); -moz-transform: rotate(-21deg); -o-transform: rotate(-21deg); -webkit-transform: rotate(-21deg); background: #6a94e0; }
div.hfr2d			{ width: 45px; height: 100px; top: 145px; left: 410px; -ms-transform: rotate(-21deg); -moz-transform: rotate(-21deg); -o-transform: rotate(-21deg); -webkit-transform: rotate(-21deg); background: #6a94e0; }
div.hfr2e			{ width: 10px; height: 60px; top: 236px; left: 436px; -ms-transform: rotate(-18deg); -moz-transform: rotate(-18deg); -o-transform: rotate(-18deg); -webkit-transform: rotate(-18deg); background: #4970ab; }
div.hfr2f			{ width: 25px; height: 180px; top: 227px; left: 437px; -ms-transform: rotate(-21deg); -moz-transform: rotate(-21deg); -o-transform: rotate(-21deg); -webkit-transform: rotate(-21deg); border-left: 2px solid #000; }

div#hair_frontr3	{  }
div.hfr3a			{ width: 72px; height: 72px; top: 222px; left: 410px; -ms-transform: rotate(36deg) skew(32deg,32deg); -moz-transform: rotate(36deg) skew(32deg,32deg); -o-transform: rotate(36deg) skew(32deg,32deg); -webkit-transform: rotate(36deg) skew(32deg,32deg); background: -ms-linear-gradient(top right, #6a94e0 60% , rgba(106, 148, 224, 0) 60%); background: -moz-linear-gradient(top right, #6a94e0 60% , rgba(106, 148, 224, 0) 60%); background: -o-linear-gradient(top right, #6a94e0 60% , rgba(106, 148, 224, 0) 60%); background: -webkit-linear-gradient(top right, #6a94e0 60% , rgba(106, 148, 224, 0) 60%); border-top: 3px solid #000; border-right: 3px solid #000; border-radius: 0 72px; }
div.hfr3b			{ width: 30px; height: 275px; top: 87px; left: 368px; overflow: hidden; -ms-transform: rotate(-19deg); -o-transform: rotate(-19deg); -webkit-transform: rotate(-19deg); -moz-transform: rotate(-19deg); border-left: 2px solid #000; }
div.hfr3b1			{ width: 12px; height: 230px; background: #6a94e0; }
div.hfr3b2			{ width: 20px; height: 190px; background: #6a94e0; }
div.hfr3b3			{ width: 12px; height: 250px; -ms-transform: rotate(2.5deg); -moz-transform: rotate(2.5deg); -o-transform: rotate(2.5deg); -webkit-transform: rotate(2.5deg); background: #4970ab; }

div#hair_frontr4	{  }
div.hfr4a			{ width: 40px; height: 130px; top: 38px; left: 333px; -ms-transform: rotate(-10deg); -moz-transform: rotate(-10deg); -o-transform: rotate(-10deg); -webkit-transform: rotate(-10deg); background: #6a94e0; }
div.hfr4b			{ width: 100px; height: 100px; top: 109px; left: 315px; -ms-transform: rotate(29deg) skew(30deg,30deg); -moz-transform: rotate(29deg) skew(30deg,30deg); -o-transform: rotate(29deg) skew(30deg,30deg); -webkit-transform: rotate(29deg) skew(30deg,30deg); background: #6a94e0; border-left: 3px solid #000; border-bottom: 3px solid #000; border-radius: 0 100px; }
div.hfr4c			{ width: 85px; height: 85px; top: 120px; left: 349px; -ms-transform: rotate(40deg) skew(35deg,35deg); -moz-transform: rotate(40deg) skew(35deg,35deg); -o-transform: rotate(40deg) skew(35deg,35deg); -webkit-transform: rotate(40deg) skew(35deg,35deg); background: #6a94e0; border-top: 4px solid #000; border-right: 4px solid #000; border-radius: 0 85px; }

/*眉毛*/
div#brows			{  }
div.brows1			{ width: 50px; height: 55px; top: 110px; left: 180px; -ms-transform: rotate(-26deg); -moz-transform: rotate(-26deg); -o-transform: rotate(-26deg); -webkit-transform: rotate(-26deg); border-top: 2px solid #000; border-right: 2px solid #000; border-radius: 0 45px; }
div.brows2			{ width: 45px; height: 77px; top: 164px; left: 344px; -ms-transform: rotate(-40deg) skew(10deg,10deg); -moz-transform: rotate(-40deg) skew(10deg,10deg); -o-transform: rotate(-40deg) skew(10deg,10deg); -webkit-transform: rotate(-40deg) skew(10deg,10deg); border-top: 2px solid #000; border-right: 2px solid #000; border-radius: 0 35px / 0 40px; }

/*嘴*/
div#mouth			{  }
div.mouth1			{ margin: -20px 0 0; }
div.mouth1a			{ width: 35px; height: 18px; top: 356px; left: 279px; background: #e4a3ab; border-radius: 0 0 15px 22px / 0 0 15px 20px; }
div.mouth1b			{ width: 10px; height: 10px; top: 357px; left: 275px; -ms-transform: rotate(-43deg); -moz-transform: rotate(-43deg); -o-transform: rotate(-43deg); -webkit-transform: rotate(-43deg); background: #b86f7a; }
div.mouth1c			{ width: 35px; height: 18px; top: 356px; left: 276px; border: 2px solid #000; border-top: 0; border-radius: 0 0 15px 22px / 0 0 15px 20px; }
div.mouth2			{ width: 55px; height: 25px; top: 333px; left: 270px; -ms-transform: rotate(10deg); -moz-transform: rotate(10deg); -o-transform: rotate(10deg); -webkit-transform: rotate(10deg); background: #f2d6be; }
div.mouth3			{ width: 10px; height: 10px; top: 350px; left: 265px; -ms-transform: rotate(-40deg); -moz-transform: rotate(-40deg); -o-transform: rotate(-40deg); -webkit-transform: rotate(-40deg); background: #f2d6be; border-left: 2px solid #000; border-bottom: 2px solid #000; border-bottom-left-radius: 12px; }
div.mouth4			{ width: 25px; height: 25px; top: 347px; left: 278px; -ms-transform: rotate(-35deg); -moz-transform: rotate(-35deg); -o-transform: rotate(-35deg); -webkit-transform: rotate(-35deg); background: #f2d6be; border-left: 2px solid #000; border-bottom: 2px solid #000; border-bottom-left-radius: 29px; }
div.draw:hover div.mouth1	{ margin: 0; }

/*眼睛*/
div#eye				{  }
div#eye_left		{  }
div.eyel1			{ width: 60px; height: 80px; top: 214px; left: 187px; background: -ms-linear-gradient(top, #d0cfdd 19px , #fff 22px); background: -moz-linear-gradient(top, #d0cfdd 19px , #fff 22px); background: -o-linear-gradient(top, #d0cfdd 19px , #fff 22px); background: -webkit-linear-gradient(top, #d0cfdd 19px , #fff 22px); border-radius: 0 50px 25px 35px / 0 30px 50px 70px; }
div.eyel2			{ width: 46px; height: 73px; top: 215px; left: 199px; background: -ms-linear-gradient(top, #2D4F34 70% , #48854D 100%); background: -moz-linear-gradient(top, #2D4F34 70% , #48854D 100%); background: -o-linear-gradient(top, #2D4F34 70% , #48854D 100%); background: -webkit-linear-gradient(top, #2D4F34 70% , #48854D 100%); border: 1.5px solid #000; border-radius: 10px 40px 20px 25px / 25px 20px 40px 40px; }
div.eyel3			{ width: 33px; height: 28px; top: 255px; left: 209px; -ms-transform: rotate(8deg); -moz-transform: rotate(8deg); -o-transform: rotate(8deg); -webkit-transform: rotate(8deg); background: -ms-linear-gradient(top, rgba(129,195,123,0) 0% , #81C37B 100%); background: -moz-linear-gradient(top, rgba(129,195,123,0) 0% , #81C37B 100%); background: -o-linear-gradient(top, rgba(129,195,123,0) 0% , #81C37B 100%); background: -webkit-linear-gradient(top, rgba(129,195,123,0) 0% , #81C37B 100%); border-radius: 0 0 12px 17px / 0 0 20px 20px; }
div.eyel4			{ width: 35px; height: 35px; top: 185px; left: 165px; -ms-transform: rotate(37deg) skew(40deg,40deg); -moz-transform: rotate(37deg) skew(40deg,40deg); -o-transform: rotate(37deg) skew(40deg,40deg); -webkit-transform: rotate(37deg) skew(40deg,40deg); background: -ms-linear-gradient(top left, rgba(0,0,0,0) 50% , #000 50%); background: -moz-linear-gradient(top left, rgba(0,0,0,0) 50% , #000 50%); background: -o-linear-gradient(top left, rgba(0,0,0,0) 50% , #000 50%); background: -webkit-linear-gradient(top left, rgba(0,0,0,0) 50% , #000 50%); }
div.eyel5			{ width: 17px; height: 17px; top: 280px; left: 200px; -ms-transform: rotate(-26deg) skew(10deg,10deg); -moz-transform: rotate(-26deg) skew(10deg,10deg); -o-transform: rotate(-26deg) skew(10deg,10deg); -webkit-transform: rotate(-26deg) skew(10deg,10deg); border-left: 2px solid #000; border-bottom: 2px solid #000; border-bottom-left-radius: 21px; }
div.eyel6			{ width: 3px; height: 5px; left: 218px; top: 259px; background: #fff; border-radius: 2px / 3px; }
div.eyel7			{ width: 17px; height: 13px; left: 197px; top: 261px; background: #fff; border-radius: 8px / 6px; }
div.eyel8			{ width: 70px; height: 10px; top: 202px; left: 180px; -ms-transform: rotate(20deg); -moz-transform: rotate(20deg); -o-transform: rotate(20deg); -webkit-transform: rotate(20deg); border-top: 2px solid #000; }
div.eyel9			{ width: 72px; height: 8px; top: 212px; left: 178px; -ms-transform: rotate(20deg); -moz-transform: rotate(20deg); -o-transform: rotate(20deg); -webkit-transform: rotate(20deg); background: #000; border: 1px solid #000; }

div#eye_right		{  }
div.eyer1			{ width: 80px; height: 70px; top: 260px; left: 348px; -ms-transform: rotate(16deg); -moz-transform: rotate(16deg); -o-transform: rotate(16deg); -webkit-transform: rotate(16deg); background: -ms-linear-gradient(top, #d0cfdd 19px , #fff 22px); background: -moz-linear-gradient(top, #d0cfdd 19px , #fff 22px); background: -o-linear-gradient(top, #d0cfdd 19px , #fff 22px); background: -webkit-linear-gradient(top, #d0cfdd 19px , #fff 22px); border-radius: 0 0 35px 30px / 0 0 60px 70px; }
div.eyer2			{ width: 63px; height: 70px; top: 255px; left: 360px; -ms-transform: rotate(16deg); -moz-transform: rotate(16deg); -o-transform: rotate(16deg); -webkit-transform: rotate(16deg); background: -ms-linear-gradient(top, #2d4f34 70% , #48854d 100%); background: -moz-linear-gradient(top, #2d4f34 70% , #48854d 100%); background: -o-linear-gradient(top, #2d4f34 70% , #48854d 100%); background: -webkit-linear-gradient(top, #2d4f34 70% , #48854d 100%); border: 1.5px solid #000; border-radius: 0 0 30px 30px / 0 0 50px 60px; }
div.eyer3			{ width: 40px; height: 28px; top: 291px; left: 364px; -ms-transform: rotate(15deg); -moz-transform: rotate(15deg); -o-transform: rotate(15deg); -webkit-transform: rotate(15deg); background: -ms-linear-gradient(top, rgba(129,195,123,0) 0% , #81c37b 100%); background: -moz-linear-gradient(top, rgba(129,195,123,0) 0% , #81c37b 100%); background: -o-linear-gradient(top, rgba(129,195,123,0) 0% , #81c37b 100%); background: -webkit-linear-gradient(top, rgba(129,195,123,0) 0% , #81c37b 100%); border-radius: 0 0 22px 18px / 0 0 25px 25px; }
div.eyer4			{ width: 30px; height: 30px; top: 250px; left: 425px; -ms-transform: rotate(-17deg) skew(-40deg,-40deg); -moz-transform: rotate(-17deg) skew(-40deg,-40deg); -o-transform: rotate(-17deg) skew(-40deg,-40deg); -webkit-transform: rotate(-17deg) skew(-40deg,-40deg); background: -ms-linear-gradient(top right, rgba(0,0,0,0) 50% , #000 50%); background: -moz-linear-gradient(top right, rgba(0,0,0,0) 50% , #000 50%); background: -o-linear-gradient(top right, rgba(0,0,0,0) 50% , #000 50%); background: -webkit-linear-gradient(top right, rgba(0,0,0,0) 50% , #000 50%); }
div.eyer5			{ width: 19px; height: 19px; top: 315px; left: 351px; -ms-transform: rotate(-25deg) skew(10deg,10deg); -moz-transform: rotate(-25deg) skew(10deg,10deg); -o-transform: rotate(-25deg) skew(10deg,10deg); -webkit-transform: rotate(-25deg) skew(10deg,10deg); border-left: 2px solid #000; border-bottom: 2px solid #000; border-bottom-left-radius: 21px; }
div.eyer6			{ width: 4px; height: 5px; top: 296px; left: 373px; background: #fff; border-radius: 2px / 3px; }
div.eyer7			{ width: 18px; height: 14px; top: 294px; left: 349px; background: #fff; border-radius: 9px / 7px; }
div.eyer8			{ width: 90px; height: 10px; top: 245px; left: 340px; -ms-transform: rotate(16deg); -moz-transform: rotate(16deg); -o-transform: rotate(16deg); -webkit-transform: rotate(16deg); border-top: 2px solid #000; }
div.eyer9			{ width: 100px; height: 10px; top: 255px; left: 340px; -ms-transform: rotate(16deg); -moz-transform: rotate(16deg); -o-transform: rotate(16deg); -webkit-transform: rotate(16deg); background: #000; border: 1px solid #000; }

/*光暈*/
div#light			{ opacity: 0.7; }
div#light div		{ background: #d1e0ff; }
div.light1			{ width: 75px; height: 75px; top: 6px; left: 109px; -ms-transform: rotate(-8deg) skew(31deg,31deg); -moz-transform: rotate(-8deg) skew(31deg,31deg); -o-transform: rotate(-8deg) skew(31deg,31deg); -webkit-transform: rotate(-8deg) skew(31deg,31deg); border-radius: 0 70px; }
div.light2			{ width: 100px; height: 25px; top: 6px; left: 137px; -ms-transform: rotate(55deg); -moz-transform: rotate(55deg); -o-transform: rotate(55deg); -webkit-transform: rotate(55deg); }
div.light3			{ width: 51px; height: 16px; top: 61px; left: 206px; -ms-transform: rotate(42deg) skew(5deg,0deg); -moz-transform: rotate(42deg) skew(5deg,0deg); -o-transform: rotate(42deg) skew(5deg,0deg); -webkit-transform: rotate(42deg) skew(5deg,0deg); }
div.light4			{ width: 60px; height: 20px; top: 2px; left: 130px; -ms-transform: rotate(36deg); -moz-transform: rotate(36deg); -o-transform: rotate(36deg); -webkit-transform: rotate(36deg); }
div.light5			{ width: 39px; height: 39px; top: 99px; left: 259px; -ms-transform: rotate(-27deg) skew(32deg,32deg); -moz-transform: rotate(-27deg) skew(32deg,32deg); -o-transform: rotate(-27deg) skew(32deg,32deg); -webkit-transform: rotate(-27deg) skew(32deg,32deg); border-radius: 0 39px; }
div.light6			{ width: 25px; height: 12px; top: 90px; left: 256px; -ms-transform: rotate(26deg) skew(25deg,0deg); -moz-transform: rotate(26deg) skew(25deg,0deg); -o-transform: rotate(26deg) skew(25deg,0deg); -webkit-transform: rotate(26deg) skew(25deg,0deg); }
div.light7			{ width: 38px; height: 7px; top: 103px; left: 276px; -ms-transform: rotate(25.5deg); -moz-transform: rotate(25.5deg); -o-transform: rotate(25.5deg); -webkit-transform: rotate(25.5deg); }
div.light8			{ width: 70px; height: 70px; top: 145px; left: 430px; -ms-transform: rotate(-35deg) skew(32deg,32deg); -moz-transform: rotate(-35deg) skew(32deg,32deg); -o-transform: rotate(-35deg) skew(32deg,32deg); -webkit-transform: rotate(-35deg) skew(32deg,32deg); border-radius: 0 70px; }
div.light9			{ width: 65px; height: 65px; top: 100px; left: 549px; -ms-transform: rotate(41.5deg) skew(28deg,28deg); -moz-transform: rotate(41.5deg) skew(28deg,28deg); -o-transform: rotate(41.5deg) skew(28deg,28deg); -webkit-transform: rotate(41.5deg) skew(28deg,28deg); border-radius: 0 65px; }
div.light10			{ width: 100px; height: 10px; top: 145px; left: 470px; -ms-transform: rotate(-7deg); -moz-transform: rotate(-7deg); -o-transform: rotate(-7deg); -webkit-transform: rotate(-7deg); }
div.light11			{ width: 50px; height: 10px; top: 141px; left: 520px; -ms-transform: rotate(-13deg); -moz-transform: rotate(-13deg); -o-transform: rotate(-13deg); -webkit-transform: rotate(-13deg); }
div.light12			{ width: 60px; height: 22px; top: 147px; left: 510px; }

/*光暈遮光片*/
div#dark			{  }
div.dark1			{ width: 22px; height: 76px; top: 60px; left: 545px; -ms-transform: rotate(-13deg); -moz-transform: rotate(-13deg); -o-transform: rotate(-13deg); -webkit-transform: rotate(-13deg); background: #6a94e0; border-radius: 0 0 22px / 0 0 76px; }
div.dark2			{ width: 18px; height: 28px; top: 176px; left: 565px; -ms-transform: rotate(10deg); -moz-transform: rotate(10deg); -o-transform: rotate(10deg); -webkit-transform: rotate(10deg); background: #6a94e0; border-radius: 0 18px 0 / 0 28px 0; }

/*手*/
div#hand			{  }
div#hand div		{ background: #f2d6be; }
div.hand1			{ width: 20px; height: 30px; top: 346px; left: 482px; -ms-transform: rotate(35deg); -moz-transform: rotate(35deg); -o-transform: rotate(35deg); -webkit-transform: rotate(35deg); }
div.hand2			{ width: 33px; height: 62px; top: 370px; left: 368px; -ms-transform: rotate(-40deg); -moz-transform: rotate(-40deg); -o-transform: rotate(-40deg); -webkit-transform: rotate(-40deg); border: 1.5px solid #000; border-radius: 25px 10px 0 0 / 30px 10px 0 0; }
div.hand3			{ width: 36px; height: 62px; top: 310px; left: 515px; -ms-transform: rotate(43deg); -moz-transform: rotate(43deg); -o-transform: rotate(43deg); -webkit-transform: rotate(43deg); border: 1.5px solid #000; border-bottom: 0; border-radius: 25px 12px 0 0 / 40px 12px 0 0; }
div.hand4			{ width: 30px; height: 120px; top: 380px; left: 462px; -ms-transform: rotate(10deg); -moz-transform: rotate(10deg); -o-transform: rotate(10deg); -webkit-transform: rotate(10deg); border-right: 1.5px solid #000; }
div.hand5			{ width: 30px; height: 30px; top: 366px; left: 471px; -ms-transform: rotate(22deg); -moz-transform: rotate(22deg); -o-transform: rotate(22deg); -webkit-transform: rotate(22deg); border-right: 1.5px solid #000; }
div.hand6			{ width: 30px; height: 14px; top: 356px; left: 480px; -ms-transform: rotate(38deg); -moz-transform: rotate(38deg); -o-transform: rotate(38deg); -webkit-transform: rotate(38deg); border-right: 1.5px solid #000; }
div.hand7			{ width: 33px; height: 33px; top: 352px; left: 450px; -ms-transform: rotate(-25deg) skew(-20deg,-20deg); -moz-transform: rotate(-25deg) skew(-20deg,-20deg); -o-transform: rotate(-25deg) skew(-20deg,-20deg); -webkit-transform: rotate(-25deg) skew(-20deg,-20deg); border-top: 2px solid #000; border-left: 2px solid #000; border-top-left-radius: 35px; }
div.hand8			{ width: 80px; height: 65px; top: 387px; left: 400px; -ms-transform: rotate(17deg) skew(17deg,18deg); -moz-transform: rotate(17deg) skew(17deg,18deg); -o-transform: rotate(17deg) skew(17deg,18deg); -webkit-transform: rotate(17deg) skew(17deg,18deg); border-top: 1px solid #000; border-left: 1px solid #000; border-radius: 70px 0 / 50px 0; }
div.hand9			{ width: 54px; height: 55px; top: 420px; left: 402px; -ms-transform: rotate(12deg) skew(10deg,10deg); -moz-transform: rotate(12deg) skew(10deg,10deg); -o-transform: rotate(12deg) skew(10deg,10deg); -webkit-transform: rotate(12deg) skew(10deg,10deg); border-top: 1px solid #000; border-left: 1px solid #000; border-radius: 52px 0 / 28px 0; }
div.hand10			{ width: 13px; height: 10px; top: 428px; left: 452px; -ms-transform: rotate(-20deg); -moz-transform: rotate(-20deg); -o-transform: rotate(-20deg); -webkit-transform: rotate(-20deg); border-top: 1.5px solid #000; }
div.hand11			{ width: 51px; height: 55px; top: 453px; left: 394px; -ms-transform: skew(15deg,14deg); -moz-transform: skew(15deg,14deg); -o-transform: skew(15deg,14deg); -webkit-transform: skew(15deg,14deg); border-top: 1px solid #000; border-left: 1px solid #000; border-radius: 48px 0 / 28px 0; }
div.hand12			{ width: 17px; height: 10px; top: 454px; left: 442px; -ms-transform: rotate(-39deg); -moz-transform: rotate(-39deg); -o-transform: rotate(-39deg); -webkit-transform: rotate(-39deg); border-top: 1.5px solid #000; }


div#bubble			{  }
div.bubble1			{ width: 200px; height: 300px; background: #fff; border-radius: 0 0 200px / 0 0 300px; }
div.bubble2			{ width: 100px; height: 100px; top: 180px; left: 30px; -ms-transform: rotate(10deg) skew(35deg,35deg); -moz-transform: rotate(10deg) skew(35deg,35deg); -o-transform: rotate(10deg) skew(35deg,35deg); -webkit-transform: rotate(10deg) skew(35deg,35deg); background: #fff; }
div.bubble3			{ width: 60px; left: 50px; top: 30px; font-size: 60px; line-height: 70px; font-family: 'Century Gothic', 'Lucida Grande', 'メイリオ', 'MS PGothic'; text-align: center; text-shadow: 4px 4px 2px #ccc; }


div.copy				{ padding: 0 0 4px; color: #444; text-shadow: 2px 2px 2px #aaa; }
a						{ color: #09f; }
a:hover					{ color: #008; }

div.hover			{ -ms-transition: all 1s; -moz-transition: all 1s; -o-transition: all 1s; -webkit-transition: all 1s; }
div.fuwafuwa_l		{ -ms-animation: fuwafuwa_l 4s infinite; -moz-animation: fuwafuwa_l 4s infinite; -o-animation: fuwafuwa_l 4s infinite; -webkit-animation: fuwafuwa_l 4s infinite; }
div.fuwafuwa_r		{ -ms-animation: fuwafuwa_r 4s infinite; -moz-animation: fuwafuwa_r 4s infinite; -o-animation: fuwafuwa_r 4s infinite; -webkit-animation: fuwafuwa_r 4s infinite; }
div.kirakira		{ -ms-animation: kirakira 0.5s infinite; -moz-animation: kirakira 0.5s infinite; -o-animation: kirakira 0.5s infinite; -webkit-animation: kirakira 0.5s infinite; }

@-ms-keyframes fuwafuwa_l {
	0%, 50%, 100% { -ms-transform: rotate(-0.5deg); }
	25%, 75% { -ms-transform: rotate(0.5deg); }
}

@-ms-keyframes fuwafuwa_r {
	0%, 50%, 100% { -ms-transform: rotate(0.5deg); }
	25%, 75% { -ms-transform: rotate(-0.5deg); }
}

@-ms-keyframes kirakira {
	0%, 50%, 100% { margin: 0; }
	25%, 75% { margin: 0 0 0 1px; }
}

@-moz-keyframes fuwafuwa_l {
	0%, 50%, 100% { -moz-transform: rotate(-0.5deg); }
	25%, 75% { -moz-transform: rotate(0.5deg); }
}

@-moz-keyframes fuwafuwa_r {
	0%, 50%, 100% { -moz-transform: rotate(0.5deg); }
	25%, 75% { -moz-transform: rotate(-0.5deg); }
}

@-moz-keyframes kirakira {
	0%, 50%, 100% { margin: 0; }
	25%, 75% { margin: 0 0 0 1px; }
}

@-o-keyframes fuwafuwa_l {
	0%, 50%, 100% { -o-transform: rotate(-0.5deg); }
	25%, 75% { -o-transform: rotate(0.5deg); }
}

@-o-keyframes fuwafuwa_r {
	0%, 50%, 100% { -o-transform: rotate(0.5deg); }
	25%, 75% { -o-transform: rotate(-0.5deg); }
}

@-o-keyframes kirakira {
	0%, 50%, 100% { margin: 0; }
	25%, 75% { margin: 0 0 0 2px; }
}

@-webkit-keyframes fuwafuwa_l {
	0%, 50%, 100% { -webkit-transform: rotate(-0.5deg); }
	25%, 75% { -webkit-transform: rotate(0.5deg); }
}

@-webkit-keyframes fuwafuwa_r {
	0%, 50%, 100% { -webkit-transform: rotate(0.5deg); }
	25%, 75% { -webkit-transform: rotate(-0.5deg); }
}

@-webkit-keyframes kirakira {
	0%, 50%, 100% { margin: 0; }
	25%, 75% { margin: 0 0 0 2px; }
}
</style>
<div id="main">
  <div id="ins">
    <div class="draw">
      <div id="bg"></div>
      <div id="hair_back">
        <div class="hb1"></div>
        <div class="hb2"></div>
        <div class="hb3"></div>
        <div class="hb4"></div>
        <div class="hb5"></div>
        <div class="hb6"></div>
        <div class="hb7"></div>
      </div>
      <div id="neck">
        <div class="neck1"></div>
        <div class="neck2"></div>
      </div>
      <div id="clothes">
        <div class="clothes1"></div>
        <div class="clothes2"></div>
        <div class="clothes3"></div>
        <div class="clothes4"></div>
        <div class="clothes5"></div>
        <div class="clothes6"></div>
        <div class="clothes7"></div>
        <div class="clothes8"></div>
        <div class="clothes9"></div>
        <div class="clothes10"></div>
        <div class="clothes11">
          <div class="clothes11a"></div>
        </div>
        <div class="clothes12">
          <div class="clothes12a"></div>
          <div class="clothes12b"></div>
        </div>
        <div class="clothes13"></div>
        <div class="clothes14"></div>
        <div class="clothes15"></div>
        <div class="clothes16">
          <div class="clothes16a"></div>
        </div>
        <div class="clothes17"></div>
      </div>
      <div id="hair_right" class="fuwafuwa_l">
        <div class="hr1"></div>
        <div class="hr2"></div>
        <div class="hr3"></div>
        <div class="hr4"></div>
        <div class="hr5"></div>
        <div class="hr6"></div>
        <div class="hr7"></div>
      </div>
      <div id="face">
        <div class="face1"></div>
        <div class="face2"></div>
        <div class="face3"></div>
        <div class="face4"></div>
        <div class="face5"></div>
        <div class="face6"></div>
        <div class="face7"></div>
        <div class="face8"></div>
        <div class="face9"></div>
        <div class="face10"></div>
        <div class="face11"></div>
        <div class="face12"></div>
        <div class="face13"></div>
        <div class="face14"></div>
        <div class="face15"></div>
        <div class="face16"></div>
        <div class="face17"></div>
        <div class="face18"></div>
      </div>
      <div id="ear">
        <div class="ear1"></div>
        <div class="ear2"></div>
      </div>
      <div id="hair_left" class="fuwafuwa_r">
        <div class="hl1"></div>
        <div class="hl2"></div>
        <div class="hl3"></div>
        <div class="hl4"></div>
        <div class="hl5"></div>
        <div class="hl6"></div>
        <div class="hl7"></div>
        <div class="hl8"></div>
        <div class="hl9"></div>
        <div class="hl10"></div>
        <div class="hl11"></div>
      </div>
      <div id="hair_front">
        <div class="hair_front">
          <div class="hf1"></div>
          <div class="hf2"></div>
        </div>
        <div id="hair_frontl1" class="fuwafuwa_l">
          <div class="hfl1a"></div>
          <div class="hfl1b"></div>
          <div class="hfl1c"></div>
          <div class="hfl1d"></div>
          <div class="hfl1e"></div>
        </div>
        <div id="hair_frontl2" class="fuwafuwa_l">
          <div class="hfl2a"></div>
          <div class="hfl2b"></div>
          <div class="hfl2c"></div>
          <div class="hfl2d"></div>
          <div class="hfl2e"></div>
        </div>
        <div id="hair_frontl3" class="fuwafuwa_r">
          <div class="hfl3a"></div>
          <div class="hfl3b"></div>
          <div class="hfl3c"></div>
          <div class="hfl3d"></div>
          <div class="hfl3e"></div>
          <div class="hfl3f"></div>
        </div>
        <div id="hair_frontl4" class="fuwafuwa_l">
          <div class="hfl4a"></div>
          <div class="hfl4b"></div>
          <div class="hfl4c"></div>
          <div class="hfl4d"></div>
          <div class="hfl4e"></div>
          <div class="hfl4f"></div>
        </div>
        <div id="hair_frontl5" class="fuwafuwa_r">
          <div class="hfl5a"></div>
          <div class="hfl5b"></div>
          <div class="hfl5c">
            <div class="hfl5c1"></div>
          </div>
        </div>
        <div id="hair_frontl6" class="fuwafuwa_l">
          <div class="hfl6a"></div>
          <div class="hfl6b"></div>
          <div class="hfl6c">
            <div class="hfl6c1"></div>
          </div>
          <div class="hfl6d"></div>
        </div>
        <div id="hair_frontr1" class="fuwafuwa_r">
          <div class="hfr1a"></div>
          <div class="hfr1b"></div>
          <div class="hfr1c"></div>
          <div class="hfr1d"></div>
        </div>
        <div id="hair_frontr2" class="fuwafuwa_r">
          <div class="hfr2a"></div>
          <div class="hfr2b"></div>
          <div class="hfr2c"></div>
          <div class="hfr2d"></div>
          <div class="hfr2e"></div>
          <div class="hfr2f"></div>
        </div>
        <div id="hair_frontr3" class="fuwafuwa_r">
          <div class="hfr3a"></div>
          <div class="hfr3b">
            <div class="hfr3b1"></div>
            <div class="hfr3b2"></div>
            <div class="hfr3b3"></div>
          </div>
        </div>
        <div id="hair_frontr4" class="fuwafuwa_r">
          <div class="hfr4a"></div>
          <div class="hfr4b"></div>
          <div class="hfr4c"></div>
        </div>
      </div>
      <div id="brows">
        <div class="brows1"></div>
        <div class="brows2"></div>
      </div>
      <div id="mouth">
        <div class="mouth1 hover">
          <div class="mouth1a"></div>
          <div class="mouth1b"></div>
          <div class="mouth1c"></div>
        </div>
        <div class="mouth2"></div>
        <div class="mouth3"></div>
        <div class="mouth4"></div>
      </div>
      <div id="eye">
        <div id="eye_left">
          <div class="eyel1"></div>
          <div class="eyel2"></div>
          <div class="eyel3"></div>
                  <div class="eyel4"></div>
          <div class="eyel5"></div>
          <div class="eyel6 kirakira"></div>
          <div class="eyel7 kirakira"></div>
          <div class="eyel8"></div>
          <div class="eyel9"></div>
        </div>
        <div id="eye_right">
          <div class="eyer1"></div>
          <div class="eyer2"></div>
          <div class="eyer3"></div>
                  <div class="eyer4"></div>
          <div class="eyer5"></div>
          <div class="eyer6 kirakira"></div>
          <div class="eyer7 kirakira"></div>
          <div class="eyer8"></div>
          <div class="eyer9"></div>
        </div>
      </div>
      <div id="light">
        <div class="light1"></div>
        <div class="light2"></div>
        <div class="light3"></div>
        <div class="light4"></div>
        <div class="light5"></div>
        <div class="light6"></div>
        <div class="light7"></div>
        <div class="light8"></div>
        <div class="light9"></div>
        <div class="light10"></div>
        <div class="light11"></div>
        <div class="light12"></div>
      </div>
      <div id="dark">
        <div class="dark1"></div>
        <div class="dark2"></div>
      </div>
      <div id="hand" class="hover">
              <div class="hand1"></div>
        <div class="hand2"></div>
        <div class="hand3"></div>
        <div class="hand4"></div>
        <div class="hand5"></div>
        <div class="hand6"></div>
        <div class="hand7"></div>
        <div class="hand8"></div>
        <div class="hand9"></div>
        <div class="hand10"></div>
        <div class="hand11"></div>
        <div class="hand12"></div>
      </div>
      <div id="bubble" class="hover">
        <div class="bubble1"></div>
        <div class="bubble2"></div>
        <div class="bubble3"><span class="red">Что</span><br />там<br />?</div>
      </div>
    </div>
  </div>
</div>
