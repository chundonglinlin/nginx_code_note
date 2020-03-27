<html>
    <head>
        <meta http-equiv=Content-Type content="text/html; charset=utf-8">
        <meta name=Generator content="Microsoft Word 15 (filtered)">
        <title>nginx-rtmp</title>
        <style>
        <!--
         /* Font Definitions */
         @font-face
            {font-family:"Cambria Math";
            panose-1:2 4 5 3 5 4 6 3 2 4;}
        @font-face
            {font-family:等线;
            panose-1:2 1 6 0 3 1 1 1 1 1;}
        @font-face
            {font-family:"等线 Light";
            panose-1:2 1 6 0 3 1 1 1 1 1;}
        @font-face
            {font-family:"\@等线";
            panose-1:2 1 6 0 3 1 1 1 1 1;}
        @font-face
            {font-family:"\@等线 Light";
            panose-1:2 1 6 0 3 1 1 1 1 1;}
         /* Style Definitions */
         p.MsoNormal, li.MsoNormal, div.MsoNormal
            {margin:0cm;
            margin-bottom:.0001pt;
            text-align:justify;
            text-justify:inter-ideograph;
            font-size:10.5pt;
            font-family:等线;}
        h1
            {mso-style-link:"标题 1 字符";
            margin-top:17.0pt;
            margin-right:0cm;
            margin-bottom:16.5pt;
            margin-left:0cm;
            text-align:justify;
            text-justify:inter-ideograph;
            line-height:240%;
            page-break-after:avoid;
            font-size:22.0pt;
            font-family:等线;}
        h2
            {mso-style-link:"标题 2 字符";
            margin-top:13.0pt;
            margin-right:0cm;
            margin-bottom:13.0pt;
            margin-left:0cm;
            text-align:justify;
            text-justify:inter-ideograph;
            line-height:173%;
            page-break-after:avoid;
            font-size:16.0pt;
            font-family:"等线 Light";}
        p.MsoToc1, li.MsoToc1, div.MsoToc1
            {margin:0cm;
            margin-bottom:.0001pt;
            text-align:justify;
            text-justify:inter-ideograph;
            font-size:10.5pt;
            font-family:等线;}
        p.MsoToc2, li.MsoToc2, div.MsoToc2
            {margin-top:0cm;
            margin-right:0cm;
            margin-bottom:0cm;
            margin-left:21.0pt;
            margin-bottom:.0001pt;
            text-align:justify;
            text-justify:inter-ideograph;
            font-size:10.5pt;
            font-family:等线;}
        p.MsoHeader, li.MsoHeader, div.MsoHeader
            {mso-style-link:"页眉 字符";
            margin:0cm;
            margin-bottom:.0001pt;
            text-align:center;
            layout-grid-mode:char;
            border:none;
            padding:0cm;
            font-size:9.0pt;
            font-family:等线;}
        p.MsoFooter, li.MsoFooter, div.MsoFooter
            {mso-style-link:"页脚 字符";
            margin:0cm;
            margin-bottom:.0001pt;
            layout-grid-mode:char;
            font-size:9.0pt;
            font-family:等线;}
        a:link, span.MsoHyperlink
            {color:blue;
            text-decoration:underline;}
        a:visited, span.MsoHyperlinkFollowed
            {color:#954F72;
            text-decoration:underline;}
        p.MsoNoSpacing, li.MsoNoSpacing, div.MsoNoSpacing
            {margin:0cm;
            margin-bottom:.0001pt;
            text-align:justify;
            text-justify:inter-ideograph;
            font-size:10.5pt;
            font-family:等线;}
        p.MsoListParagraph, li.MsoListParagraph, div.MsoListParagraph
            {margin:0cm;
            margin-bottom:.0001pt;
            text-align:justify;
            text-justify:inter-ideograph;
            text-indent:21.0pt;
            font-size:10.5pt;
            font-family:等线;}
        p.MsoTocHeading, li.MsoTocHeading, div.MsoTocHeading
            {margin-top:12.0pt;
            margin-right:0cm;
            margin-bottom:0cm;
            margin-left:0cm;
            margin-bottom:.0001pt;
            line-height:107%;
            page-break-after:avoid;
            font-size:16.0pt;
            font-family:"等线 Light";
            color:#2F5496;}
        span.1
            {mso-style-name:"标题 1 字符";
            mso-style-link:"标题 1";
            font-weight:bold;}
        span.a
            {mso-style-name:"页眉 字符";
            mso-style-link:页眉;}
        span.a0
            {mso-style-name:"页脚 字符";
            mso-style-link:页脚;}
        span.2
            {mso-style-name:"标题 2 字符";
            mso-style-link:"标题 2";
            font-family:"等线 Light";
            font-weight:bold;}
        .MsoChpDefault
            {font-family:等线;}
         /* Page Definitions */
         @page WordSection1
            {size:595.3pt 841.9pt;
            margin:72.0pt 90.0pt 72.0pt 90.0pt;
            layout-grid:15.6pt;}
        div.WordSection1
            {page:WordSection1;}
         /* List Definitions */
         ol
            {margin-bottom:0cm;}
        ul
            {margin-bottom:0cm;}
        -->
        </style>
    </head>

    <body lang=ZH-CN link=blue vlink=purple style='text-justify-trim:punctuation'>
        <div class=WordSection1 style='layout-grid:15.6pt'>
            <h1>
                <a name="_Toc462219403"></a>
                <a name="_Toc26097915">nginx-rtmp(wiki整理)</a>
            </h1>

            <p class=MsoNormal>
                <span lang=EN>&nbsp;&nbsp; </span>
                <span lang=EN-US>
                    <a href="https://mp.weixin.qq.com/s/LVNz4aFYYDaoCU3trE9bxg">
                        <span style='font-family:"Segoe UI",sans-serif;color:#095EAB;background:white'>https://mp.weixin.qq.com/s/LVNz4aFYYDaoCU3trE9bxg</span>
                    </a>
                </span>
                <span lang=EN>&nbsp;&nbsp;&nbsp; PingOS</span>
                <span style='font-family:宋体'>基于Nginx媒体服务</span>
            </p>

            <h1>
                <a name="_Toc26097995"></a>
                <a name="_Toc462219560">常用的直播平台网站</a>
            </h1>

            <p class=MsoNormal>
                <span lang=EN>&nbsp;&nbsp; </span>
                <span lang=EN-US>
                    <a href="http://ossrs.net/srs.release/releases/">
                        <span style='font-family:"Segoe UI",sans-serif;color:#095EAB;background:white'>http://ossrs.net/srs.release/releases/</span>
                    </a>
                </span>
                <span lang=EN>&nbsp;&nbsp;&nbsp; SRS</span>
                <span style='font-family:宋体'>官网</span>
            </p>

            <p class=MsoNormal>
                <span lang=EN>&nbsp;&nbsp; </span><span lang=EN-US>
                    <a href="https://github.com/arut/nginx-rtmp-module">
                        <span lang=EN>https://github.com/arut/nginx-rtmp-module</span>
                    </a>
                </span>
                <span lang=EN>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; nginx rtmp</span>
                <span style='font-family:宋体'>官网</span>
            </p>

            <p class=MsoNormal>
                <span lang=EN>&nbsp;&nbsp; </span>
                <span lang=EN-US>
                    <a href="https://www.qcloud.com/product/LVB.html">
                        <span lang=EN>https://www.qcloud.com/product/LVB.html</span>
                    </a>
                </span>
                <span lang=EN>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>
                <span style='font-family:宋体'>腾讯云直播</span>
            </p>

            <p class=MsoNormal>
                <span lang=EN>&nbsp;&nbsp; </span>
                <span lang=EN-US>
                    <a href="https://www.aliyun.com/product/live?spm=5176.7960203.237031.164.Ve6N2d">
                        <span lang=EN>https://www.aliyun.com/product/live?spm=5176.7960203.237031.164.Ve6N2d</span>
                    </a>
                </span>
                <span lang=EN> </span>
                <span style='font-family:宋体'>阿里云直播</span>
            </p>

            <p class=MsoNormal>
                <span lang=EN>&nbsp;&nbsp; </span>
                <span lang=EN-US>
                    <a href="https://bce.baidu.com/product/lss.html">
                        <span lang=EN>https://bce.baidu.com/product/lss.html</span>
                    </a>
                </span>
                <span lang=EN>&nbsp;&nbsp; </span>
                <span style='font-family:宋体'>百度云直播</span>
            </p>

            <p class=MsoNormal>
                <span lang=EN>&nbsp;&nbsp; </span>
                <span lang=EN-US>
                    <a href="http://www.lecloud.com/zh-cn/product/live.html">
                        <span lang=EN>http://www.lecloud.com/zh-cn/product/live.html</span>
                    </a>
                </span>
                <span lang=EN>&nbsp;&nbsp; </span>
                <span style='font-family:宋体'>乐视云直播</span>
            </p>

            <p class=MsoNormal>
                <span lang=EN>&nbsp;&nbsp; </span>
                <span lang=EN-US>
                    <a href="https://www.upyun.com/products/video.html">
                        <span lang=EN>https://www.upyun.com/products/video.html</span>
                    </a>
                </span>
                <span lang=EN>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>
                <span style='font-family:宋体'>又拍云直播</span>
            </p>

            <p class=MsoNormal>
                <span lang=EN>&nbsp;&nbsp; </span>
                <span lang=EN-US>
                    <a href="http://www.qiniu.com/products/live">
                        <span lang=EN>http://www.qiniu.com/products/live</span>
                    </a>
                </span>
                <span lang=EN>&nbsp;&nbsp;&nbsp;&nbsp; </span>
                <span style='font-family:宋体'>七牛云直播</span>
            </p>

            <p class=MsoNormal>
                <span lang=EN>&nbsp;&nbsp; </span>
                <span lang=EN-US>
                    <a href="http://xycdn.com/site/solution">
                        <span lang=EN>http://xycdn.com/site/solution</span>
                    </a>
                </span>
                <span lang=EN>&nbsp;&nbsp; </span>
                <span style='font-family:宋体'>星域云</span>
                <span lang=EN>(</span><span style='font-family:宋体'>讯雷旗下的公司</span><span lang=EN>)</span>
            </p>

            <p class=MsoNormal>
                <span lang=EN>&nbsp;&nbsp; </span>
                <span lang=EN-US>
                    <a href="http://www.easydarwin.org">
                        <span lang=EN>http://www.easydarwin.org</span>
                    </a>
                </span>
                <span lang=EN>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; RTSP</span>
                <span style='font-family:宋体'>开源平台</span>
            </p>

            <p class=MsoNormal>
                <span lang=EN>&nbsp;&nbsp; </span>
                <span lang=EN-US>
                    <a href="http://www.easydarwin.org">
                        <span lang=EN>https://www.liveqing.com/</span>
                    </a>
                </span>
                <span lang=EN>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;LiveQing</span>
                <span style='font-family:宋体'>开源平台</span>
            </p>

            <p class=MsoNormal>
                <span lang=EN-US>&nbsp;</span>
            </p>
        </div>
    </body>
</html>
