# ngx-bitmap-render

api:

```ts
export type NgxOptions = Record<string, unknown>;

export enum ChartType {
  AdvancedPieChartComponent = 'AdvancedPieChartComponent',
  AreaChartComponent = 'AreaChartComponent',
  AreaChartNormalizedComponent = 'AreaChartNormalizedComponent',
  AreaChartStackedComponent = 'AreaChartStackedComponent',
  BarHorizontal2DComponent = 'BarHorizontal2DComponent',
  BarHorizontalComponent = 'BarHorizontalComponent',
  BarHorizontalNormalizedComponent = 'BarHorizontalNormalizedComponent',
  BarHorizontalStackedComponent = 'BarHorizontalStackedComponent',
  BarVertical2DComponent = 'BarVertical2DComponent',
  BarVerticalComponent = 'BarVerticalComponent',
  BarVerticalNormalizedComponent = 'BarVerticalNormalizedComponent',
  BarVerticalStackedComponent = 'BarVerticalStackedComponent',
  BoxChartComponent = 'BoxChartComponent',
  BubbleChartComponent = 'BubbleChartComponent',
  GaugeComponent = 'GaugeComponent',
  HeatMapComponent = 'HeatMapComponent',
  LineChartComponent = 'LineChartComponent',
  LinearGaugeComponent = 'LinearGaugeComponent',
  NumberCardComponent = 'NumberCardComponent',
  PieChartComponent = 'PieChartComponent',
  PieGridComponent = 'PieGridComponent',
  PolarChartComponent = 'PolarChartComponent',
  SankeyComponent = 'SankeyComponent',
  TreeMapComponent = 'TreeMapComponent',
}

export interface ChartParam {
  type: ChartType;
  externalCSS?: string;
  ngxOptions?: Partial<NgxOptions>;
}

export type IndexApiParam = Partial<ChartParam>;

const exampleJson: IndexApiParam = {
  type: 'BarVerticalComponent',
  externalCSS: '',
  ngxOptions: {
    results: [
      {
        name: 'Germany',
        value: 40632,
        extra: {
          code: 'de',
        },
      },
      {
        name: 'United States',
        value: 50000,
        extra: {
          code: 'us',
        },
      },
      {
        name: 'France',
        value: 36745,
        extra: {
          code: 'fr',
        },
      },
      {
        name: 'United Kingdom',
        value: 36240,
        extra: {
          code: 'uk',
        },
      },
      {
        name: 'Spain',
        value: 33000,
        extra: {
          code: 'es',
        },
      },
      {
        name: 'Italy',
        value: 35800,
        extra: {
          code: 'it',
        },
      },
    ],
    showGridLines: true,
    showLegend: true,
    showXAxisLabel: true,
    showYAxisLabel: true,
    xAxisLabel: 'xAxisLabel',
    yAxisLabel: 'yAxisLabel',
    xAxis: true,
    yAxis: true,
    legend: true,
    view: [700, 300],
    animations: false,
  },
};
```

[example.http](docs/example.http)

