# geofacet_seoul
geofacet chart for Seoul with [geofacet](https://hafen.github.io/geofacet/) package

```
ggplot(pop) +
  geom_line(aes(yq, pph), color="red") +
  facet_geo(~ gu, grid=seoul_grid, label='name') +
  theme(axis.text.x = element_text(angle=45, hjust=1),
        text = element_text(size=6)) +
  labs(title="서울시 자치구별 세대당 인구 추이",
       caption="Data Source: stat.seoul.go.kr",
       x="연도(분기별)",
       y="세대당 인구")
```

![geofacet](https://github.com/yonghah/geofacet_seoul/blob/master/.Rproj.user/shared/notebooks/1B0E306D-geofacet_seoul/1/s/ctawik7ymslp0/00000a.png)
