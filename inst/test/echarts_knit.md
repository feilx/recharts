
```r
library(knitr)
knit2html("echarts_knit.Rmd", template = "tempt.html")
```



```r
library(recharts)
```

# Line Plot

```r
eLine(iris[, 1:4])
```


<div id='ID_20131024085116_68187' style='height:500px;border:1px solid #ccc;padding:10px;'></div>
    
<script type='text/javascript'>
    // Step:3 conifg ECharts's path, link to echarts.js from current page.
    require.config({
        paths:{ 
            'echarts': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/bar' : 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/line': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/scatter': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/k': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/pie': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/map': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/force': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/radar': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map'
        }
    });
    
    // Step:4 require echarts and use it in the callback.
    require(
        [
            'echarts',
            'echarts/chart/bar',
            'echarts/chart/line',
            'echarts/chart/scatter',
            'echarts/chart/k',
            'echarts/chart/pie',
            'echarts/chart/map',
            'echarts/chart/force',
            'echarts/chart/radar'
        ],
        function(ec) {
            var EChart_ID_20131024085116_68187 = ec.init(document.getElementById('ID_20131024085116_68187'));
            var option_ID_20131024085116_68187 = {
	"legend" : {
		"data" : [
			"Sepal.Length",
			"Sepal.Width",
			"Petal.Length",
			"Petal.Width"
		]
	},
	"toolbox" : {
		"show" : true,
		"feature" : {
			"mark" : true,
			"dataView" : true,
			"magicType" : [
				"line",
				"bar"
			],
			"restore" : true,
			"saveAsImage" : true
		}
	},
	"tooltip" : {
		"trigger" : "axis"
	},
	"xAxis" : {
		"type" : "category",
		"boundaryGap" : false,
		"data" : [
			"1",
			"2",
			"3",
			"4",
			"5",
			"6",
			"7",
			"8",
			"9",
			"10",
			"11",
			"12",
			"13",
			"14",
			"15",
			"16",
			"17",
			"18",
			"19",
			"20",
			"21",
			"22",
			"23",
			"24",
			"25",
			"26",
			"27",
			"28",
			"29",
			"30",
			"31",
			"32",
			"33",
			"34",
			"35",
			"36",
			"37",
			"38",
			"39",
			"40",
			"41",
			"42",
			"43",
			"44",
			"45",
			"46",
			"47",
			"48",
			"49",
			"50",
			"51",
			"52",
			"53",
			"54",
			"55",
			"56",
			"57",
			"58",
			"59",
			"60",
			"61",
			"62",
			"63",
			"64",
			"65",
			"66",
			"67",
			"68",
			"69",
			"70",
			"71",
			"72",
			"73",
			"74",
			"75",
			"76",
			"77",
			"78",
			"79",
			"80",
			"81",
			"82",
			"83",
			"84",
			"85",
			"86",
			"87",
			"88",
			"89",
			"90",
			"91",
			"92",
			"93",
			"94",
			"95",
			"96",
			"97",
			"98",
			"99",
			"100",
			"101",
			"102",
			"103",
			"104",
			"105",
			"106",
			"107",
			"108",
			"109",
			"110",
			"111",
			"112",
			"113",
			"114",
			"115",
			"116",
			"117",
			"118",
			"119",
			"120",
			"121",
			"122",
			"123",
			"124",
			"125",
			"126",
			"127",
			"128",
			"129",
			"130",
			"131",
			"132",
			"133",
			"134",
			"135",
			"136",
			"137",
			"138",
			"139",
			"140",
			"141",
			"142",
			"143",
			"144",
			"145",
			"146",
			"147",
			"148",
			"149",
			"150"
		]
	},
	"series" : [
		{
			"type" : "line",
			"name" : "Sepal.Length",
			"data" : [
				5.1,
				4.9,
				4.7,
				4.6,
				5,
				5.4,
				4.6,
				5,
				4.4,
				4.9,
				5.4,
				4.8,
				4.8,
				4.3,
				5.8,
				5.7,
				5.4,
				5.1,
				5.7,
				5.1,
				5.4,
				5.1,
				4.6,
				5.1,
				4.8,
				5,
				5,
				5.2,
				5.2,
				4.7,
				4.8,
				5.4,
				5.2,
				5.5,
				4.9,
				5,
				5.5,
				4.9,
				4.4,
				5.1,
				5,
				4.5,
				4.4,
				5,
				5.1,
				4.8,
				5.1,
				4.6,
				5.3,
				5,
				7,
				6.4,
				6.9,
				5.5,
				6.5,
				5.7,
				6.3,
				4.9,
				6.6,
				5.2,
				5,
				5.9,
				6,
				6.1,
				5.6,
				6.7,
				5.6,
				5.8,
				6.2,
				5.6,
				5.9,
				6.1,
				6.3,
				6.1,
				6.4,
				6.6,
				6.8,
				6.7,
				6,
				5.7,
				5.5,
				5.5,
				5.8,
				6,
				5.4,
				6,
				6.7,
				6.3,
				5.6,
				5.5,
				5.5,
				6.1,
				5.8,
				5,
				5.6,
				5.7,
				5.7,
				6.2,
				5.1,
				5.7,
				6.3,
				5.8,
				7.1,
				6.3,
				6.5,
				7.6,
				4.9,
				7.3,
				6.7,
				7.2,
				6.5,
				6.4,
				6.8,
				5.7,
				5.8,
				6.4,
				6.5,
				7.7,
				7.7,
				6,
				6.9,
				5.6,
				7.7,
				6.3,
				6.7,
				7.2,
				6.2,
				6.1,
				6.4,
				7.2,
				7.4,
				7.9,
				6.4,
				6.3,
				6.1,
				7.7,
				6.3,
				6.4,
				6,
				6.9,
				6.7,
				6.9,
				5.8,
				6.8,
				6.7,
				6.7,
				6.3,
				6.5,
				6.2,
				5.9
			]
		},
		{
			"type" : "line",
			"name" : "Sepal.Width",
			"data" : [
				3.5,
				3,
				3.2,
				3.1,
				3.6,
				3.9,
				3.4,
				3.4,
				2.9,
				3.1,
				3.7,
				3.4,
				3,
				3,
				4,
				4.4,
				3.9,
				3.5,
				3.8,
				3.8,
				3.4,
				3.7,
				3.6,
				3.3,
				3.4,
				3,
				3.4,
				3.5,
				3.4,
				3.2,
				3.1,
				3.4,
				4.1,
				4.2,
				3.1,
				3.2,
				3.5,
				3.6,
				3,
				3.4,
				3.5,
				2.3,
				3.2,
				3.5,
				3.8,
				3,
				3.8,
				3.2,
				3.7,
				3.3,
				3.2,
				3.2,
				3.1,
				2.3,
				2.8,
				2.8,
				3.3,
				2.4,
				2.9,
				2.7,
				2,
				3,
				2.2,
				2.9,
				2.9,
				3.1,
				3,
				2.7,
				2.2,
				2.5,
				3.2,
				2.8,
				2.5,
				2.8,
				2.9,
				3,
				2.8,
				3,
				2.9,
				2.6,
				2.4,
				2.4,
				2.7,
				2.7,
				3,
				3.4,
				3.1,
				2.3,
				3,
				2.5,
				2.6,
				3,
				2.6,
				2.3,
				2.7,
				3,
				2.9,
				2.9,
				2.5,
				2.8,
				3.3,
				2.7,
				3,
				2.9,
				3,
				3,
				2.5,
				2.9,
				2.5,
				3.6,
				3.2,
				2.7,
				3,
				2.5,
				2.8,
				3.2,
				3,
				3.8,
				2.6,
				2.2,
				3.2,
				2.8,
				2.8,
				2.7,
				3.3,
				3.2,
				2.8,
				3,
				2.8,
				3,
				2.8,
				3.8,
				2.8,
				2.8,
				2.6,
				3,
				3.4,
				3.1,
				3,
				3.1,
				3.1,
				3.1,
				2.7,
				3.2,
				3.3,
				3,
				2.5,
				3,
				3.4,
				3
			]
		},
		{
			"type" : "line",
			"name" : "Petal.Length",
			"data" : [
				1.4,
				1.4,
				1.3,
				1.5,
				1.4,
				1.7,
				1.4,
				1.5,
				1.4,
				1.5,
				1.5,
				1.6,
				1.4,
				1.1,
				1.2,
				1.5,
				1.3,
				1.4,
				1.7,
				1.5,
				1.7,
				1.5,
				1,
				1.7,
				1.9,
				1.6,
				1.6,
				1.5,
				1.4,
				1.6,
				1.6,
				1.5,
				1.5,
				1.4,
				1.5,
				1.2,
				1.3,
				1.4,
				1.3,
				1.5,
				1.3,
				1.3,
				1.3,
				1.6,
				1.9,
				1.4,
				1.6,
				1.4,
				1.5,
				1.4,
				4.7,
				4.5,
				4.9,
				4,
				4.6,
				4.5,
				4.7,
				3.3,
				4.6,
				3.9,
				3.5,
				4.2,
				4,
				4.7,
				3.6,
				4.4,
				4.5,
				4.1,
				4.5,
				3.9,
				4.8,
				4,
				4.9,
				4.7,
				4.3,
				4.4,
				4.8,
				5,
				4.5,
				3.5,
				3.8,
				3.7,
				3.9,
				5.1,
				4.5,
				4.5,
				4.7,
				4.4,
				4.1,
				4,
				4.4,
				4.6,
				4,
				3.3,
				4.2,
				4.2,
				4.2,
				4.3,
				3,
				4.1,
				6,
				5.1,
				5.9,
				5.6,
				5.8,
				6.6,
				4.5,
				6.3,
				5.8,
				6.1,
				5.1,
				5.3,
				5.5,
				5,
				5.1,
				5.3,
				5.5,
				6.7,
				6.9,
				5,
				5.7,
				4.9,
				6.7,
				4.9,
				5.7,
				6,
				4.8,
				4.9,
				5.6,
				5.8,
				6.1,
				6.4,
				5.6,
				5.1,
				5.6,
				6.1,
				5.6,
				5.5,
				4.8,
				5.4,
				5.6,
				5.1,
				5.1,
				5.9,
				5.7,
				5.2,
				5,
				5.2,
				5.4,
				5.1
			]
		},
		{
			"type" : "line",
			"name" : "Petal.Width",
			"data" : [
				0.2,
				0.2,
				0.2,
				0.2,
				0.2,
				0.4,
				0.3,
				0.2,
				0.2,
				0.1,
				0.2,
				0.2,
				0.1,
				0.1,
				0.2,
				0.4,
				0.4,
				0.3,
				0.3,
				0.3,
				0.2,
				0.4,
				0.2,
				0.5,
				0.2,
				0.2,
				0.4,
				0.2,
				0.2,
				0.2,
				0.2,
				0.4,
				0.1,
				0.2,
				0.2,
				0.2,
				0.2,
				0.1,
				0.2,
				0.2,
				0.3,
				0.3,
				0.2,
				0.6,
				0.4,
				0.3,
				0.2,
				0.2,
				0.2,
				0.2,
				1.4,
				1.5,
				1.5,
				1.3,
				1.5,
				1.3,
				1.6,
				1,
				1.3,
				1.4,
				1,
				1.5,
				1,
				1.4,
				1.3,
				1.4,
				1.5,
				1,
				1.5,
				1.1,
				1.8,
				1.3,
				1.5,
				1.2,
				1.3,
				1.4,
				1.4,
				1.7,
				1.5,
				1,
				1.1,
				1,
				1.2,
				1.6,
				1.5,
				1.6,
				1.5,
				1.3,
				1.3,
				1.3,
				1.2,
				1.4,
				1.2,
				1,
				1.3,
				1.2,
				1.3,
				1.3,
				1.1,
				1.3,
				2.5,
				1.9,
				2.1,
				1.8,
				2.2,
				2.1,
				1.7,
				1.8,
				1.8,
				2.5,
				2,
				1.9,
				2.1,
				2,
				2.4,
				2.3,
				1.8,
				2.2,
				2.3,
				1.5,
				2.3,
				2,
				2,
				1.8,
				2.1,
				1.8,
				1.8,
				1.8,
				2.1,
				1.6,
				1.9,
				2,
				2.2,
				1.5,
				1.4,
				2.3,
				2.4,
				1.8,
				1.8,
				2.1,
				2.4,
				2.3,
				1.9,
				2.3,
				2.5,
				2.3,
				1.9,
				2,
				2.3,
				1.8
			]
		}
	]
}            
            EChart_ID_20131024085116_68187.setOption(option_ID_20131024085116_68187);
        }
    );
</script>
	

```r
eLine(iris[, 1:4], opt = list(dataZoom = list(show = TRUE, end = 35)))
```


<div id='ID_20131024085116_68190' style='height:500px;border:1px solid #ccc;padding:10px;'></div>
    
<script type='text/javascript'>
    // Step:3 conifg ECharts's path, link to echarts.js from current page.
    require.config({
        paths:{ 
            'echarts': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/bar' : 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/line': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/scatter': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/k': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/pie': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/map': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/force': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/radar': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map'
        }
    });
    
    // Step:4 require echarts and use it in the callback.
    require(
        [
            'echarts',
            'echarts/chart/bar',
            'echarts/chart/line',
            'echarts/chart/scatter',
            'echarts/chart/k',
            'echarts/chart/pie',
            'echarts/chart/map',
            'echarts/chart/force',
            'echarts/chart/radar'
        ],
        function(ec) {
            var EChart_ID_20131024085116_68190 = ec.init(document.getElementById('ID_20131024085116_68190'));
            var option_ID_20131024085116_68190 = {
	"dataZoom" : {
		"show" : true,
		"end" : 35
	},
	"legend" : {
		"data" : [
			"Sepal.Length",
			"Sepal.Width",
			"Petal.Length",
			"Petal.Width"
		]
	},
	"toolbox" : {
		"show" : true,
		"feature" : {
			"mark" : true,
			"dataView" : true,
			"magicType" : [
				"line",
				"bar"
			],
			"restore" : true,
			"saveAsImage" : true
		}
	},
	"tooltip" : {
		"trigger" : "axis"
	},
	"xAxis" : {
		"type" : "category",
		"boundaryGap" : false,
		"data" : [
			"1",
			"2",
			"3",
			"4",
			"5",
			"6",
			"7",
			"8",
			"9",
			"10",
			"11",
			"12",
			"13",
			"14",
			"15",
			"16",
			"17",
			"18",
			"19",
			"20",
			"21",
			"22",
			"23",
			"24",
			"25",
			"26",
			"27",
			"28",
			"29",
			"30",
			"31",
			"32",
			"33",
			"34",
			"35",
			"36",
			"37",
			"38",
			"39",
			"40",
			"41",
			"42",
			"43",
			"44",
			"45",
			"46",
			"47",
			"48",
			"49",
			"50",
			"51",
			"52",
			"53",
			"54",
			"55",
			"56",
			"57",
			"58",
			"59",
			"60",
			"61",
			"62",
			"63",
			"64",
			"65",
			"66",
			"67",
			"68",
			"69",
			"70",
			"71",
			"72",
			"73",
			"74",
			"75",
			"76",
			"77",
			"78",
			"79",
			"80",
			"81",
			"82",
			"83",
			"84",
			"85",
			"86",
			"87",
			"88",
			"89",
			"90",
			"91",
			"92",
			"93",
			"94",
			"95",
			"96",
			"97",
			"98",
			"99",
			"100",
			"101",
			"102",
			"103",
			"104",
			"105",
			"106",
			"107",
			"108",
			"109",
			"110",
			"111",
			"112",
			"113",
			"114",
			"115",
			"116",
			"117",
			"118",
			"119",
			"120",
			"121",
			"122",
			"123",
			"124",
			"125",
			"126",
			"127",
			"128",
			"129",
			"130",
			"131",
			"132",
			"133",
			"134",
			"135",
			"136",
			"137",
			"138",
			"139",
			"140",
			"141",
			"142",
			"143",
			"144",
			"145",
			"146",
			"147",
			"148",
			"149",
			"150"
		]
	},
	"series" : [
		{
			"type" : "line",
			"name" : "Sepal.Length",
			"data" : [
				5.1,
				4.9,
				4.7,
				4.6,
				5,
				5.4,
				4.6,
				5,
				4.4,
				4.9,
				5.4,
				4.8,
				4.8,
				4.3,
				5.8,
				5.7,
				5.4,
				5.1,
				5.7,
				5.1,
				5.4,
				5.1,
				4.6,
				5.1,
				4.8,
				5,
				5,
				5.2,
				5.2,
				4.7,
				4.8,
				5.4,
				5.2,
				5.5,
				4.9,
				5,
				5.5,
				4.9,
				4.4,
				5.1,
				5,
				4.5,
				4.4,
				5,
				5.1,
				4.8,
				5.1,
				4.6,
				5.3,
				5,
				7,
				6.4,
				6.9,
				5.5,
				6.5,
				5.7,
				6.3,
				4.9,
				6.6,
				5.2,
				5,
				5.9,
				6,
				6.1,
				5.6,
				6.7,
				5.6,
				5.8,
				6.2,
				5.6,
				5.9,
				6.1,
				6.3,
				6.1,
				6.4,
				6.6,
				6.8,
				6.7,
				6,
				5.7,
				5.5,
				5.5,
				5.8,
				6,
				5.4,
				6,
				6.7,
				6.3,
				5.6,
				5.5,
				5.5,
				6.1,
				5.8,
				5,
				5.6,
				5.7,
				5.7,
				6.2,
				5.1,
				5.7,
				6.3,
				5.8,
				7.1,
				6.3,
				6.5,
				7.6,
				4.9,
				7.3,
				6.7,
				7.2,
				6.5,
				6.4,
				6.8,
				5.7,
				5.8,
				6.4,
				6.5,
				7.7,
				7.7,
				6,
				6.9,
				5.6,
				7.7,
				6.3,
				6.7,
				7.2,
				6.2,
				6.1,
				6.4,
				7.2,
				7.4,
				7.9,
				6.4,
				6.3,
				6.1,
				7.7,
				6.3,
				6.4,
				6,
				6.9,
				6.7,
				6.9,
				5.8,
				6.8,
				6.7,
				6.7,
				6.3,
				6.5,
				6.2,
				5.9
			]
		},
		{
			"type" : "line",
			"name" : "Sepal.Width",
			"data" : [
				3.5,
				3,
				3.2,
				3.1,
				3.6,
				3.9,
				3.4,
				3.4,
				2.9,
				3.1,
				3.7,
				3.4,
				3,
				3,
				4,
				4.4,
				3.9,
				3.5,
				3.8,
				3.8,
				3.4,
				3.7,
				3.6,
				3.3,
				3.4,
				3,
				3.4,
				3.5,
				3.4,
				3.2,
				3.1,
				3.4,
				4.1,
				4.2,
				3.1,
				3.2,
				3.5,
				3.6,
				3,
				3.4,
				3.5,
				2.3,
				3.2,
				3.5,
				3.8,
				3,
				3.8,
				3.2,
				3.7,
				3.3,
				3.2,
				3.2,
				3.1,
				2.3,
				2.8,
				2.8,
				3.3,
				2.4,
				2.9,
				2.7,
				2,
				3,
				2.2,
				2.9,
				2.9,
				3.1,
				3,
				2.7,
				2.2,
				2.5,
				3.2,
				2.8,
				2.5,
				2.8,
				2.9,
				3,
				2.8,
				3,
				2.9,
				2.6,
				2.4,
				2.4,
				2.7,
				2.7,
				3,
				3.4,
				3.1,
				2.3,
				3,
				2.5,
				2.6,
				3,
				2.6,
				2.3,
				2.7,
				3,
				2.9,
				2.9,
				2.5,
				2.8,
				3.3,
				2.7,
				3,
				2.9,
				3,
				3,
				2.5,
				2.9,
				2.5,
				3.6,
				3.2,
				2.7,
				3,
				2.5,
				2.8,
				3.2,
				3,
				3.8,
				2.6,
				2.2,
				3.2,
				2.8,
				2.8,
				2.7,
				3.3,
				3.2,
				2.8,
				3,
				2.8,
				3,
				2.8,
				3.8,
				2.8,
				2.8,
				2.6,
				3,
				3.4,
				3.1,
				3,
				3.1,
				3.1,
				3.1,
				2.7,
				3.2,
				3.3,
				3,
				2.5,
				3,
				3.4,
				3
			]
		},
		{
			"type" : "line",
			"name" : "Petal.Length",
			"data" : [
				1.4,
				1.4,
				1.3,
				1.5,
				1.4,
				1.7,
				1.4,
				1.5,
				1.4,
				1.5,
				1.5,
				1.6,
				1.4,
				1.1,
				1.2,
				1.5,
				1.3,
				1.4,
				1.7,
				1.5,
				1.7,
				1.5,
				1,
				1.7,
				1.9,
				1.6,
				1.6,
				1.5,
				1.4,
				1.6,
				1.6,
				1.5,
				1.5,
				1.4,
				1.5,
				1.2,
				1.3,
				1.4,
				1.3,
				1.5,
				1.3,
				1.3,
				1.3,
				1.6,
				1.9,
				1.4,
				1.6,
				1.4,
				1.5,
				1.4,
				4.7,
				4.5,
				4.9,
				4,
				4.6,
				4.5,
				4.7,
				3.3,
				4.6,
				3.9,
				3.5,
				4.2,
				4,
				4.7,
				3.6,
				4.4,
				4.5,
				4.1,
				4.5,
				3.9,
				4.8,
				4,
				4.9,
				4.7,
				4.3,
				4.4,
				4.8,
				5,
				4.5,
				3.5,
				3.8,
				3.7,
				3.9,
				5.1,
				4.5,
				4.5,
				4.7,
				4.4,
				4.1,
				4,
				4.4,
				4.6,
				4,
				3.3,
				4.2,
				4.2,
				4.2,
				4.3,
				3,
				4.1,
				6,
				5.1,
				5.9,
				5.6,
				5.8,
				6.6,
				4.5,
				6.3,
				5.8,
				6.1,
				5.1,
				5.3,
				5.5,
				5,
				5.1,
				5.3,
				5.5,
				6.7,
				6.9,
				5,
				5.7,
				4.9,
				6.7,
				4.9,
				5.7,
				6,
				4.8,
				4.9,
				5.6,
				5.8,
				6.1,
				6.4,
				5.6,
				5.1,
				5.6,
				6.1,
				5.6,
				5.5,
				4.8,
				5.4,
				5.6,
				5.1,
				5.1,
				5.9,
				5.7,
				5.2,
				5,
				5.2,
				5.4,
				5.1
			]
		},
		{
			"type" : "line",
			"name" : "Petal.Width",
			"data" : [
				0.2,
				0.2,
				0.2,
				0.2,
				0.2,
				0.4,
				0.3,
				0.2,
				0.2,
				0.1,
				0.2,
				0.2,
				0.1,
				0.1,
				0.2,
				0.4,
				0.4,
				0.3,
				0.3,
				0.3,
				0.2,
				0.4,
				0.2,
				0.5,
				0.2,
				0.2,
				0.4,
				0.2,
				0.2,
				0.2,
				0.2,
				0.4,
				0.1,
				0.2,
				0.2,
				0.2,
				0.2,
				0.1,
				0.2,
				0.2,
				0.3,
				0.3,
				0.2,
				0.6,
				0.4,
				0.3,
				0.2,
				0.2,
				0.2,
				0.2,
				1.4,
				1.5,
				1.5,
				1.3,
				1.5,
				1.3,
				1.6,
				1,
				1.3,
				1.4,
				1,
				1.5,
				1,
				1.4,
				1.3,
				1.4,
				1.5,
				1,
				1.5,
				1.1,
				1.8,
				1.3,
				1.5,
				1.2,
				1.3,
				1.4,
				1.4,
				1.7,
				1.5,
				1,
				1.1,
				1,
				1.2,
				1.6,
				1.5,
				1.6,
				1.5,
				1.3,
				1.3,
				1.3,
				1.2,
				1.4,
				1.2,
				1,
				1.3,
				1.2,
				1.3,
				1.3,
				1.1,
				1.3,
				2.5,
				1.9,
				2.1,
				1.8,
				2.2,
				2.1,
				1.7,
				1.8,
				1.8,
				2.5,
				2,
				1.9,
				2.1,
				2,
				2.4,
				2.3,
				1.8,
				2.2,
				2.3,
				1.5,
				2.3,
				2,
				2,
				1.8,
				2.1,
				1.8,
				1.8,
				1.8,
				2.1,
				1.6,
				1.9,
				2,
				2.2,
				1.5,
				1.4,
				2.3,
				2.4,
				1.8,
				1.8,
				2.1,
				2.4,
				2.3,
				1.9,
				2.3,
				2.5,
				2.3,
				1.9,
				2,
				2.3,
				1.8
			]
		}
	]
}            
            EChart_ID_20131024085116_68190.setOption(option_ID_20131024085116_68190);
        }
    );
</script>
	


# Area Plot

```r
eArea(iris[, 1:4])
```


<div id='ID_20131024085116_68195' style='height:500px;border:1px solid #ccc;padding:10px;'></div>
    
<script type='text/javascript'>
    // Step:3 conifg ECharts's path, link to echarts.js from current page.
    require.config({
        paths:{ 
            'echarts': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/bar' : 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/line': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/scatter': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/k': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/pie': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/map': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/force': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/radar': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map'
        }
    });
    
    // Step:4 require echarts and use it in the callback.
    require(
        [
            'echarts',
            'echarts/chart/bar',
            'echarts/chart/line',
            'echarts/chart/scatter',
            'echarts/chart/k',
            'echarts/chart/pie',
            'echarts/chart/map',
            'echarts/chart/force',
            'echarts/chart/radar'
        ],
        function(ec) {
            var EChart_ID_20131024085116_68195 = ec.init(document.getElementById('ID_20131024085116_68195'));
            var option_ID_20131024085116_68195 = {
	"series" : [
		{
			"stack" : "SUM",
			"itemStyle" : {
				"normal" : {
					"areaStyle" : {
						"type" : "default"
					}
				}
			},
			"type" : "line",
			"name" : "Sepal.Length",
			"data" : [
				5.1,
				4.9,
				4.7,
				4.6,
				5,
				5.4,
				4.6,
				5,
				4.4,
				4.9,
				5.4,
				4.8,
				4.8,
				4.3,
				5.8,
				5.7,
				5.4,
				5.1,
				5.7,
				5.1,
				5.4,
				5.1,
				4.6,
				5.1,
				4.8,
				5,
				5,
				5.2,
				5.2,
				4.7,
				4.8,
				5.4,
				5.2,
				5.5,
				4.9,
				5,
				5.5,
				4.9,
				4.4,
				5.1,
				5,
				4.5,
				4.4,
				5,
				5.1,
				4.8,
				5.1,
				4.6,
				5.3,
				5,
				7,
				6.4,
				6.9,
				5.5,
				6.5,
				5.7,
				6.3,
				4.9,
				6.6,
				5.2,
				5,
				5.9,
				6,
				6.1,
				5.6,
				6.7,
				5.6,
				5.8,
				6.2,
				5.6,
				5.9,
				6.1,
				6.3,
				6.1,
				6.4,
				6.6,
				6.8,
				6.7,
				6,
				5.7,
				5.5,
				5.5,
				5.8,
				6,
				5.4,
				6,
				6.7,
				6.3,
				5.6,
				5.5,
				5.5,
				6.1,
				5.8,
				5,
				5.6,
				5.7,
				5.7,
				6.2,
				5.1,
				5.7,
				6.3,
				5.8,
				7.1,
				6.3,
				6.5,
				7.6,
				4.9,
				7.3,
				6.7,
				7.2,
				6.5,
				6.4,
				6.8,
				5.7,
				5.8,
				6.4,
				6.5,
				7.7,
				7.7,
				6,
				6.9,
				5.6,
				7.7,
				6.3,
				6.7,
				7.2,
				6.2,
				6.1,
				6.4,
				7.2,
				7.4,
				7.9,
				6.4,
				6.3,
				6.1,
				7.7,
				6.3,
				6.4,
				6,
				6.9,
				6.7,
				6.9,
				5.8,
				6.8,
				6.7,
				6.7,
				6.3,
				6.5,
				6.2,
				5.9
			]
		},
		{
			"stack" : "SUM",
			"itemStyle" : {
				"normal" : {
					"areaStyle" : {
						"type" : "default"
					}
				}
			},
			"type" : "line",
			"name" : "Sepal.Width",
			"data" : [
				3.5,
				3,
				3.2,
				3.1,
				3.6,
				3.9,
				3.4,
				3.4,
				2.9,
				3.1,
				3.7,
				3.4,
				3,
				3,
				4,
				4.4,
				3.9,
				3.5,
				3.8,
				3.8,
				3.4,
				3.7,
				3.6,
				3.3,
				3.4,
				3,
				3.4,
				3.5,
				3.4,
				3.2,
				3.1,
				3.4,
				4.1,
				4.2,
				3.1,
				3.2,
				3.5,
				3.6,
				3,
				3.4,
				3.5,
				2.3,
				3.2,
				3.5,
				3.8,
				3,
				3.8,
				3.2,
				3.7,
				3.3,
				3.2,
				3.2,
				3.1,
				2.3,
				2.8,
				2.8,
				3.3,
				2.4,
				2.9,
				2.7,
				2,
				3,
				2.2,
				2.9,
				2.9,
				3.1,
				3,
				2.7,
				2.2,
				2.5,
				3.2,
				2.8,
				2.5,
				2.8,
				2.9,
				3,
				2.8,
				3,
				2.9,
				2.6,
				2.4,
				2.4,
				2.7,
				2.7,
				3,
				3.4,
				3.1,
				2.3,
				3,
				2.5,
				2.6,
				3,
				2.6,
				2.3,
				2.7,
				3,
				2.9,
				2.9,
				2.5,
				2.8,
				3.3,
				2.7,
				3,
				2.9,
				3,
				3,
				2.5,
				2.9,
				2.5,
				3.6,
				3.2,
				2.7,
				3,
				2.5,
				2.8,
				3.2,
				3,
				3.8,
				2.6,
				2.2,
				3.2,
				2.8,
				2.8,
				2.7,
				3.3,
				3.2,
				2.8,
				3,
				2.8,
				3,
				2.8,
				3.8,
				2.8,
				2.8,
				2.6,
				3,
				3.4,
				3.1,
				3,
				3.1,
				3.1,
				3.1,
				2.7,
				3.2,
				3.3,
				3,
				2.5,
				3,
				3.4,
				3
			]
		},
		{
			"stack" : "SUM",
			"itemStyle" : {
				"normal" : {
					"areaStyle" : {
						"type" : "default"
					}
				}
			},
			"type" : "line",
			"name" : "Petal.Length",
			"data" : [
				1.4,
				1.4,
				1.3,
				1.5,
				1.4,
				1.7,
				1.4,
				1.5,
				1.4,
				1.5,
				1.5,
				1.6,
				1.4,
				1.1,
				1.2,
				1.5,
				1.3,
				1.4,
				1.7,
				1.5,
				1.7,
				1.5,
				1,
				1.7,
				1.9,
				1.6,
				1.6,
				1.5,
				1.4,
				1.6,
				1.6,
				1.5,
				1.5,
				1.4,
				1.5,
				1.2,
				1.3,
				1.4,
				1.3,
				1.5,
				1.3,
				1.3,
				1.3,
				1.6,
				1.9,
				1.4,
				1.6,
				1.4,
				1.5,
				1.4,
				4.7,
				4.5,
				4.9,
				4,
				4.6,
				4.5,
				4.7,
				3.3,
				4.6,
				3.9,
				3.5,
				4.2,
				4,
				4.7,
				3.6,
				4.4,
				4.5,
				4.1,
				4.5,
				3.9,
				4.8,
				4,
				4.9,
				4.7,
				4.3,
				4.4,
				4.8,
				5,
				4.5,
				3.5,
				3.8,
				3.7,
				3.9,
				5.1,
				4.5,
				4.5,
				4.7,
				4.4,
				4.1,
				4,
				4.4,
				4.6,
				4,
				3.3,
				4.2,
				4.2,
				4.2,
				4.3,
				3,
				4.1,
				6,
				5.1,
				5.9,
				5.6,
				5.8,
				6.6,
				4.5,
				6.3,
				5.8,
				6.1,
				5.1,
				5.3,
				5.5,
				5,
				5.1,
				5.3,
				5.5,
				6.7,
				6.9,
				5,
				5.7,
				4.9,
				6.7,
				4.9,
				5.7,
				6,
				4.8,
				4.9,
				5.6,
				5.8,
				6.1,
				6.4,
				5.6,
				5.1,
				5.6,
				6.1,
				5.6,
				5.5,
				4.8,
				5.4,
				5.6,
				5.1,
				5.1,
				5.9,
				5.7,
				5.2,
				5,
				5.2,
				5.4,
				5.1
			]
		},
		{
			"stack" : "SUM",
			"itemStyle" : {
				"normal" : {
					"areaStyle" : {
						"type" : "default"
					}
				}
			},
			"type" : "line",
			"name" : "Petal.Width",
			"data" : [
				0.2,
				0.2,
				0.2,
				0.2,
				0.2,
				0.4,
				0.3,
				0.2,
				0.2,
				0.1,
				0.2,
				0.2,
				0.1,
				0.1,
				0.2,
				0.4,
				0.4,
				0.3,
				0.3,
				0.3,
				0.2,
				0.4,
				0.2,
				0.5,
				0.2,
				0.2,
				0.4,
				0.2,
				0.2,
				0.2,
				0.2,
				0.4,
				0.1,
				0.2,
				0.2,
				0.2,
				0.2,
				0.1,
				0.2,
				0.2,
				0.3,
				0.3,
				0.2,
				0.6,
				0.4,
				0.3,
				0.2,
				0.2,
				0.2,
				0.2,
				1.4,
				1.5,
				1.5,
				1.3,
				1.5,
				1.3,
				1.6,
				1,
				1.3,
				1.4,
				1,
				1.5,
				1,
				1.4,
				1.3,
				1.4,
				1.5,
				1,
				1.5,
				1.1,
				1.8,
				1.3,
				1.5,
				1.2,
				1.3,
				1.4,
				1.4,
				1.7,
				1.5,
				1,
				1.1,
				1,
				1.2,
				1.6,
				1.5,
				1.6,
				1.5,
				1.3,
				1.3,
				1.3,
				1.2,
				1.4,
				1.2,
				1,
				1.3,
				1.2,
				1.3,
				1.3,
				1.1,
				1.3,
				2.5,
				1.9,
				2.1,
				1.8,
				2.2,
				2.1,
				1.7,
				1.8,
				1.8,
				2.5,
				2,
				1.9,
				2.1,
				2,
				2.4,
				2.3,
				1.8,
				2.2,
				2.3,
				1.5,
				2.3,
				2,
				2,
				1.8,
				2.1,
				1.8,
				1.8,
				1.8,
				2.1,
				1.6,
				1.9,
				2,
				2.2,
				1.5,
				1.4,
				2.3,
				2.4,
				1.8,
				1.8,
				2.1,
				2.4,
				2.3,
				1.9,
				2.3,
				2.5,
				2.3,
				1.9,
				2,
				2.3,
				1.8
			]
		}
	],
	"legend" : {
		"data" : [
			"Sepal.Length",
			"Sepal.Width",
			"Petal.Length",
			"Petal.Width"
		]
	},
	"toolbox" : {
		"show" : true,
		"feature" : {
			"mark" : true,
			"dataView" : true,
			"magicType" : [
				"line",
				"bar"
			],
			"restore" : true,
			"saveAsImage" : true
		}
	},
	"tooltip" : {
		"trigger" : "axis"
	},
	"xAxis" : {
		"type" : "category",
		"boundaryGap" : false,
		"data" : [
			"1",
			"2",
			"3",
			"4",
			"5",
			"6",
			"7",
			"8",
			"9",
			"10",
			"11",
			"12",
			"13",
			"14",
			"15",
			"16",
			"17",
			"18",
			"19",
			"20",
			"21",
			"22",
			"23",
			"24",
			"25",
			"26",
			"27",
			"28",
			"29",
			"30",
			"31",
			"32",
			"33",
			"34",
			"35",
			"36",
			"37",
			"38",
			"39",
			"40",
			"41",
			"42",
			"43",
			"44",
			"45",
			"46",
			"47",
			"48",
			"49",
			"50",
			"51",
			"52",
			"53",
			"54",
			"55",
			"56",
			"57",
			"58",
			"59",
			"60",
			"61",
			"62",
			"63",
			"64",
			"65",
			"66",
			"67",
			"68",
			"69",
			"70",
			"71",
			"72",
			"73",
			"74",
			"75",
			"76",
			"77",
			"78",
			"79",
			"80",
			"81",
			"82",
			"83",
			"84",
			"85",
			"86",
			"87",
			"88",
			"89",
			"90",
			"91",
			"92",
			"93",
			"94",
			"95",
			"96",
			"97",
			"98",
			"99",
			"100",
			"101",
			"102",
			"103",
			"104",
			"105",
			"106",
			"107",
			"108",
			"109",
			"110",
			"111",
			"112",
			"113",
			"114",
			"115",
			"116",
			"117",
			"118",
			"119",
			"120",
			"121",
			"122",
			"123",
			"124",
			"125",
			"126",
			"127",
			"128",
			"129",
			"130",
			"131",
			"132",
			"133",
			"134",
			"135",
			"136",
			"137",
			"138",
			"139",
			"140",
			"141",
			"142",
			"143",
			"144",
			"145",
			"146",
			"147",
			"148",
			"149",
			"150"
		]
	}
}            
            EChart_ID_20131024085116_68195.setOption(option_ID_20131024085116_68195);
        }
    );
</script>
	


# Scatter Plot

```r
ePoints(iris[, 3:5])
```


<div id='ID_20131024085116_68200' style='height:500px;border:1px solid #ccc;padding:10px;'></div>
    
<script type='text/javascript'>
    // Step:3 conifg ECharts's path, link to echarts.js from current page.
    require.config({
        paths:{ 
            'echarts': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/bar' : 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/line': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/scatter': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/k': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/pie': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/map': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/force': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/radar': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map'
        }
    });
    
    // Step:4 require echarts and use it in the callback.
    require(
        [
            'echarts',
            'echarts/chart/bar',
            'echarts/chart/line',
            'echarts/chart/scatter',
            'echarts/chart/k',
            'echarts/chart/pie',
            'echarts/chart/map',
            'echarts/chart/force',
            'echarts/chart/radar'
        ],
        function(ec) {
            var EChart_ID_20131024085116_68200 = ec.init(document.getElementById('ID_20131024085116_68200'));
            var option_ID_20131024085116_68200 = {
	"toolbox" : {
		"show" : true,
		"feature" : {
			"mark" : true,
			"dataView" : true,
			"dataZoom" : true,
			"restore" : true,
			"saveAsImage" : true
		}
	},
	"tooltip" : {
		"trigger" : "item"
	},
	"xAxis" : {
		"type" : "value",
		"power" : 1,
		"precision" : 1,
		"scale" : true
	},
	"yAxis" : {
		"type" : "value",
		"power" : 1,
		"precision" : 1,
		"scale" : true
	},
	"legend" : {
		"data" : [
			"setosa",
			"versicolor",
			"virginica"
		]
	},
	"series" : [
		{
			"type" : "scatter",
			"name" : "setosa",
			"data" : [
				[
					1.4,
					0.2
				],
				[
					1.4,
					0.2
				],
				[
					1.3,
					0.2
				],
				[
					1.5,
					0.2
				],
				[
					1.4,
					0.2
				],
				[
					1.7,
					0.4
				],
				[
					1.4,
					0.3
				],
				[
					1.5,
					0.2
				],
				[
					1.4,
					0.2
				],
				[
					1.5,
					0.1
				],
				[
					1.5,
					0.2
				],
				[
					1.6,
					0.2
				],
				[
					1.4,
					0.1
				],
				[
					1.1,
					0.1
				],
				[
					1.2,
					0.2
				],
				[
					1.5,
					0.4
				],
				[
					1.3,
					0.4
				],
				[
					1.4,
					0.3
				],
				[
					1.7,
					0.3
				],
				[
					1.5,
					0.3
				],
				[
					1.7,
					0.2
				],
				[
					1.5,
					0.4
				],
				[
					1,
					0.2
				],
				[
					1.7,
					0.5
				],
				[
					1.9,
					0.2
				],
				[
					1.6,
					0.2
				],
				[
					1.6,
					0.4
				],
				[
					1.5,
					0.2
				],
				[
					1.4,
					0.2
				],
				[
					1.6,
					0.2
				],
				[
					1.6,
					0.2
				],
				[
					1.5,
					0.4
				],
				[
					1.5,
					0.1
				],
				[
					1.4,
					0.2
				],
				[
					1.5,
					0.2
				],
				[
					1.2,
					0.2
				],
				[
					1.3,
					0.2
				],
				[
					1.4,
					0.1
				],
				[
					1.3,
					0.2
				],
				[
					1.5,
					0.2
				],
				[
					1.3,
					0.3
				],
				[
					1.3,
					0.3
				],
				[
					1.3,
					0.2
				],
				[
					1.6,
					0.6
				],
				[
					1.9,
					0.4
				],
				[
					1.4,
					0.3
				],
				[
					1.6,
					0.2
				],
				[
					1.4,
					0.2
				],
				[
					1.5,
					0.2
				],
				[
					1.4,
					0.2
				]
			]
		},
		{
			"type" : "scatter",
			"name" : "versicolor",
			"data" : [
				[
					4.7,
					1.4
				],
				[
					4.5,
					1.5
				],
				[
					4.9,
					1.5
				],
				[
					4,
					1.3
				],
				[
					4.6,
					1.5
				],
				[
					4.5,
					1.3
				],
				[
					4.7,
					1.6
				],
				[
					3.3,
					1
				],
				[
					4.6,
					1.3
				],
				[
					3.9,
					1.4
				],
				[
					3.5,
					1
				],
				[
					4.2,
					1.5
				],
				[
					4,
					1
				],
				[
					4.7,
					1.4
				],
				[
					3.6,
					1.3
				],
				[
					4.4,
					1.4
				],
				[
					4.5,
					1.5
				],
				[
					4.1,
					1
				],
				[
					4.5,
					1.5
				],
				[
					3.9,
					1.1
				],
				[
					4.8,
					1.8
				],
				[
					4,
					1.3
				],
				[
					4.9,
					1.5
				],
				[
					4.7,
					1.2
				],
				[
					4.3,
					1.3
				],
				[
					4.4,
					1.4
				],
				[
					4.8,
					1.4
				],
				[
					5,
					1.7
				],
				[
					4.5,
					1.5
				],
				[
					3.5,
					1
				],
				[
					3.8,
					1.1
				],
				[
					3.7,
					1
				],
				[
					3.9,
					1.2
				],
				[
					5.1,
					1.6
				],
				[
					4.5,
					1.5
				],
				[
					4.5,
					1.6
				],
				[
					4.7,
					1.5
				],
				[
					4.4,
					1.3
				],
				[
					4.1,
					1.3
				],
				[
					4,
					1.3
				],
				[
					4.4,
					1.2
				],
				[
					4.6,
					1.4
				],
				[
					4,
					1.2
				],
				[
					3.3,
					1
				],
				[
					4.2,
					1.3
				],
				[
					4.2,
					1.2
				],
				[
					4.2,
					1.3
				],
				[
					4.3,
					1.3
				],
				[
					3,
					1.1
				],
				[
					4.1,
					1.3
				]
			]
		},
		{
			"type" : "scatter",
			"name" : "virginica",
			"data" : [
				[
					6,
					2.5
				],
				[
					5.1,
					1.9
				],
				[
					5.9,
					2.1
				],
				[
					5.6,
					1.8
				],
				[
					5.8,
					2.2
				],
				[
					6.6,
					2.1
				],
				[
					4.5,
					1.7
				],
				[
					6.3,
					1.8
				],
				[
					5.8,
					1.8
				],
				[
					6.1,
					2.5
				],
				[
					5.1,
					2
				],
				[
					5.3,
					1.9
				],
				[
					5.5,
					2.1
				],
				[
					5,
					2
				],
				[
					5.1,
					2.4
				],
				[
					5.3,
					2.3
				],
				[
					5.5,
					1.8
				],
				[
					6.7,
					2.2
				],
				[
					6.9,
					2.3
				],
				[
					5,
					1.5
				],
				[
					5.7,
					2.3
				],
				[
					4.9,
					2
				],
				[
					6.7,
					2
				],
				[
					4.9,
					1.8
				],
				[
					5.7,
					2.1
				],
				[
					6,
					1.8
				],
				[
					4.8,
					1.8
				],
				[
					4.9,
					1.8
				],
				[
					5.6,
					2.1
				],
				[
					5.8,
					1.6
				],
				[
					6.1,
					1.9
				],
				[
					6.4,
					2
				],
				[
					5.6,
					2.2
				],
				[
					5.1,
					1.5
				],
				[
					5.6,
					1.4
				],
				[
					6.1,
					2.3
				],
				[
					5.6,
					2.4
				],
				[
					5.5,
					1.8
				],
				[
					4.8,
					1.8
				],
				[
					5.4,
					2.1
				],
				[
					5.6,
					2.4
				],
				[
					5.1,
					2.3
				],
				[
					5.1,
					1.9
				],
				[
					5.9,
					2.3
				],
				[
					5.7,
					2.5
				],
				[
					5.2,
					2.3
				],
				[
					5,
					1.9
				],
				[
					5.2,
					2
				],
				[
					5.4,
					2.3
				],
				[
					5.1,
					1.8
				]
			]
		}
	]
}            
            EChart_ID_20131024085116_68200.setOption(option_ID_20131024085116_68200);
        }
    );
</script>
	


# Pie Plot

```r
x = sample(4)
names(x) = LETTERS[1:4]
ePie(iris[, 3:5])
```


<div id='ID_20131024085116_68215' style='height:500px;border:1px solid #ccc;padding:10px;'></div>
    
<script type='text/javascript'>
    // Step:3 conifg ECharts's path, link to echarts.js from current page.
    require.config({
        paths:{ 
            'echarts': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/bar' : 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/line': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/scatter': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/k': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/pie': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/map': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/force': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/radar': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map'
        }
    });
    
    // Step:4 require echarts and use it in the callback.
    require(
        [
            'echarts',
            'echarts/chart/bar',
            'echarts/chart/line',
            'echarts/chart/scatter',
            'echarts/chart/k',
            'echarts/chart/pie',
            'echarts/chart/map',
            'echarts/chart/force',
            'echarts/chart/radar'
        ],
        function(ec) {
            var EChart_ID_20131024085116_68215 = ec.init(document.getElementById('ID_20131024085116_68215'));
            var option_ID_20131024085116_68215 = {
	"toolbox" : {
		"show" : true,
		"feature" : {
			"mark" : true,
			"dataView" : true,
			"restore" : true,
			"saveAsImage" : true
		}
	},
	"tooltip" : {
		"trigger" : "item",
		"formatter" : "{b} : {c} ({d}%)"
	},
	"legend" : {
		"orient" : "vertical",
		"x" : "left",
		"data" : [
			"Petal.Length",
			"Petal.Width",
			"Species"
		]
	},
	"calculable" : true,
	"series" : [
		{
			"type" : "pie",
			"data" : [
				{
					"value.Petal.Length" : 1.4,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.4,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.3,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.5,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.4,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.7,
					"value.Petal.Width" : 0.4,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.4,
					"value.Petal.Width" : 0.3,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.5,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.4,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.5,
					"value.Petal.Width" : 0.1,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.5,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.6,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.4,
					"value.Petal.Width" : 0.1,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.1,
					"value.Petal.Width" : 0.1,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.2,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.5,
					"value.Petal.Width" : 0.4,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.3,
					"value.Petal.Width" : 0.4,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.4,
					"value.Petal.Width" : 0.3,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.7,
					"value.Petal.Width" : 0.3,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.5,
					"value.Petal.Width" : 0.3,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.7,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.5,
					"value.Petal.Width" : 0.4,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.7,
					"value.Petal.Width" : 0.5,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.9,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.6,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.6,
					"value.Petal.Width" : 0.4,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.5,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.4,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.6,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.6,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.5,
					"value.Petal.Width" : 0.4,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.5,
					"value.Petal.Width" : 0.1,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.4,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.5,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.2,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.3,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.4,
					"value.Petal.Width" : 0.1,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.3,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.5,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.3,
					"value.Petal.Width" : 0.3,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.3,
					"value.Petal.Width" : 0.3,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.3,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.6,
					"value.Petal.Width" : 0.6,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.9,
					"value.Petal.Width" : 0.4,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.4,
					"value.Petal.Width" : 0.3,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.6,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 1.4,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 1.5,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 1.4,
					"value.Petal.Width" : 0.2,
					"value.Species" : "setosa",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 4.7,
					"value.Petal.Width" : 1.4,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.5,
					"value.Petal.Width" : 1.5,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.9,
					"value.Petal.Width" : 1.5,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 4,
					"value.Petal.Width" : 1.3,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.6,
					"value.Petal.Width" : 1.5,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.5,
					"value.Petal.Width" : 1.3,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 4.7,
					"value.Petal.Width" : 1.6,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 3.3,
					"value.Petal.Width" : 1,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.6,
					"value.Petal.Width" : 1.3,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 3.9,
					"value.Petal.Width" : 1.4,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 3.5,
					"value.Petal.Width" : 1,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.2,
					"value.Petal.Width" : 1.5,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 4,
					"value.Petal.Width" : 1,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.7,
					"value.Petal.Width" : 1.4,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 3.6,
					"value.Petal.Width" : 1.3,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 4.4,
					"value.Petal.Width" : 1.4,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.5,
					"value.Petal.Width" : 1.5,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.1,
					"value.Petal.Width" : 1,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 4.5,
					"value.Petal.Width" : 1.5,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 3.9,
					"value.Petal.Width" : 1.1,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.8,
					"value.Petal.Width" : 1.8,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 4,
					"value.Petal.Width" : 1.3,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.9,
					"value.Petal.Width" : 1.5,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.7,
					"value.Petal.Width" : 1.2,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 4.3,
					"value.Petal.Width" : 1.3,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.4,
					"value.Petal.Width" : 1.4,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.8,
					"value.Petal.Width" : 1.4,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5,
					"value.Petal.Width" : 1.7,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.5,
					"value.Petal.Width" : 1.5,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 3.5,
					"value.Petal.Width" : 1,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 3.8,
					"value.Petal.Width" : 1.1,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 3.7,
					"value.Petal.Width" : 1,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 3.9,
					"value.Petal.Width" : 1.2,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5.1,
					"value.Petal.Width" : 1.6,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.5,
					"value.Petal.Width" : 1.5,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.5,
					"value.Petal.Width" : 1.6,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 4.7,
					"value.Petal.Width" : 1.5,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.4,
					"value.Petal.Width" : 1.3,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.1,
					"value.Petal.Width" : 1.3,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 4,
					"value.Petal.Width" : 1.3,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.4,
					"value.Petal.Width" : 1.2,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.6,
					"value.Petal.Width" : 1.4,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 4,
					"value.Petal.Width" : 1.2,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 3.3,
					"value.Petal.Width" : 1,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.2,
					"value.Petal.Width" : 1.3,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 4.2,
					"value.Petal.Width" : 1.2,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.2,
					"value.Petal.Width" : 1.3,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.3,
					"value.Petal.Width" : 1.3,
					"value.Species" : "versicolor",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 3,
					"value.Petal.Width" : 1.1,
					"value.Species" : "versicolor",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.1,
					"value.Petal.Width" : 1.3,
					"value.Species" : "versicolor",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 6,
					"value.Petal.Width" : 2.5,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5.1,
					"value.Petal.Width" : 1.9,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 5.9,
					"value.Petal.Width" : 2.1,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 5.6,
					"value.Petal.Width" : 1.8,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5.8,
					"value.Petal.Width" : 2.2,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 6.6,
					"value.Petal.Width" : 2.1,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.5,
					"value.Petal.Width" : 1.7,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 6.3,
					"value.Petal.Width" : 1.8,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 5.8,
					"value.Petal.Width" : 1.8,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 6.1,
					"value.Petal.Width" : 2.5,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5.1,
					"value.Petal.Width" : 2,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 5.3,
					"value.Petal.Width" : 1.9,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 5.5,
					"value.Petal.Width" : 2.1,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5,
					"value.Petal.Width" : 2,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 5.1,
					"value.Petal.Width" : 2.4,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 5.3,
					"value.Petal.Width" : 2.3,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5.5,
					"value.Petal.Width" : 1.8,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 6.7,
					"value.Petal.Width" : 2.2,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 6.9,
					"value.Petal.Width" : 2.3,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5,
					"value.Petal.Width" : 1.5,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 5.7,
					"value.Petal.Width" : 2.3,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.9,
					"value.Petal.Width" : 2,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 6.7,
					"value.Petal.Width" : 2,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.9,
					"value.Petal.Width" : 1.8,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 5.7,
					"value.Petal.Width" : 2.1,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 6,
					"value.Petal.Width" : 1.8,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.8,
					"value.Petal.Width" : 1.8,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 4.9,
					"value.Petal.Width" : 1.8,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5.6,
					"value.Petal.Width" : 2.1,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 5.8,
					"value.Petal.Width" : 1.6,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 6.1,
					"value.Petal.Width" : 1.9,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 6.4,
					"value.Petal.Width" : 2,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 5.6,
					"value.Petal.Width" : 2.2,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 5.1,
					"value.Petal.Width" : 1.5,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5.6,
					"value.Petal.Width" : 1.4,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 6.1,
					"value.Petal.Width" : 2.3,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 5.6,
					"value.Petal.Width" : 2.4,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5.5,
					"value.Petal.Width" : 1.8,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 4.8,
					"value.Petal.Width" : 1.8,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 5.4,
					"value.Petal.Width" : 2.1,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5.6,
					"value.Petal.Width" : 2.4,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 5.1,
					"value.Petal.Width" : 2.3,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 5.1,
					"value.Petal.Width" : 1.9,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5.9,
					"value.Petal.Width" : 2.3,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 5.7,
					"value.Petal.Width" : 2.5,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 5.2,
					"value.Petal.Width" : 2.3,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5,
					"value.Petal.Width" : 1.9,
					"value.Species" : "virginica",
					"name" : "Species"
				},
				{
					"value.Petal.Length" : 5.2,
					"value.Petal.Width" : 2,
					"value.Species" : "virginica",
					"name" : "Petal.Length"
				},
				{
					"value.Petal.Length" : 5.4,
					"value.Petal.Width" : 2.3,
					"value.Species" : "virginica",
					"name" : "Petal.Width"
				},
				{
					"value.Petal.Length" : 5.1,
					"value.Petal.Width" : 1.8,
					"value.Species" : "virginica",
					"name" : "Species"
				}
			]
		}
	]
}            
            EChart_ID_20131024085116_68215.setOption(option_ID_20131024085116_68215);
        }
    );
</script>
	


# Bar Plot

```r
eBar(iris[1:5, 1:4])
```


<div id='ID_20131024085116_68218' style='height:500px;border:1px solid #ccc;padding:10px;'></div>
    
<script type='text/javascript'>
    // Step:3 conifg ECharts's path, link to echarts.js from current page.
    require.config({
        paths:{ 
            'echarts': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/bar' : 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/line': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/scatter': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/k': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/pie': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/map': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/force': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map',
            'echarts/chart/radar': 'http://efe.baidu.com/echarts/doc/example/www/js/echarts-map'
        }
    });
    
    // Step:4 require echarts and use it in the callback.
    require(
        [
            'echarts',
            'echarts/chart/bar',
            'echarts/chart/line',
            'echarts/chart/scatter',
            'echarts/chart/k',
            'echarts/chart/pie',
            'echarts/chart/map',
            'echarts/chart/force',
            'echarts/chart/radar'
        ],
        function(ec) {
            var EChart_ID_20131024085116_68218 = ec.init(document.getElementById('ID_20131024085116_68218'));
            var option_ID_20131024085116_68218 = {
	"legend" : {
		"data" : [
			"Sepal.Length",
			"Sepal.Width",
			"Petal.Length",
			"Petal.Width"
		]
	},
	"toolbox" : {
		"show" : true,
		"feature" : {
			"mark" : true,
			"dataView" : true,
			"magicType" : [
				"line",
				"bar"
			],
			"restore" : true,
			"saveAsImage" : true
		}
	},
	"tooltip" : {
		"trigger" : "axis"
	},
	"xAxis" : {
		"type" : "category",
		"data" : [
			"1",
			"2",
			"3",
			"4",
			"5"
		]
	},
	"series" : [
		{
			"type" : "bar",
			"name" : "Sepal.Length",
			"data" : [
				5.1,
				4.9,
				4.7,
				4.6,
				5
			]
		},
		{
			"type" : "ba