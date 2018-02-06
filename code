# pl_league_trend
# R 
# Code to create plots which show league trend for six best teams in premier league

# I filter data and create six table for each teams  
arsenal <- filter(pl, team == 'Arsenal')
city <- filter(pl, team == 'Manchester City')
chelsea <- filter(pl, team == 'Chelsea')
united <- filter(pl, team == 'Manchester United')
liverpool <- filter(pl, team == 'Liverpool')
tottenham <- filter(pl, team == 'Tottenham')

# then plots for teams. For each I used diffrent line color.

arsenal_p <-ggplot(arsenal, aes(x = nb, y = place))+
  geom_point()+
  stat_smooth(se=FALSE, color='red')+
  ylim(20,1)+
  ylab("Miejsce")+
  ggtitle("Arsenal")+
  theme_bw()+
  theme(plot.title = element_text(hjust=0.5), axis.text.x=element_blank(), axis.title.x=element_blank())

city_p <- ggplot(city, aes(x = nb, y = place))+
  geom_point()+
  stat_smooth(se=FALSE, color='sky blue')+
  ylim(20,1)+
  ylab("Miejsce")+
  ggtitle("Manchester City")+
  theme_bw()+
  theme(plot.title = element_text(hjust=0.5), axis.text.x=element_blank(), axis.title.x=element_blank())
  
chelsea_p <- ggplot(chelsea, aes(x = nb, y = place))+
  geom_point()+
  stat_smooth(se=FALSE, color='blue')+
  ylim(20,1)+
  ylab("Miejsce")+
  ggtitle("Chelsea")+
  theme_bw()+
  theme(plot.title = element_text(hjust=0.5), axis.text.x=element_blank(), axis.title.x=element_blank())

united_p <- ggplot(united, aes(x = nb, y = place))+
  geom_point()+
  stat_smooth(se=FALSE, color='red')+
  ylim(20,1)+
  ylab("Miejsce")+
  ggtitle("Manchester United")+
  theme_bw()+
  theme(plot.title = element_text(hjust=0.5), axis.text.x=element_blank(), axis.title.x=element_blank())

liverpool_p <- ggplot(liverpool, aes(x = nb, y = place))+
  geom_point()+
  stat_smooth(se=FALSE, color='red')+
  ylim(20,1)+
  ylab("Miejsce")+
  ggtitle("Liverpool")+
  theme_bw()+
  theme(plot.title = element_text(hjust=0.5), axis.text.x=element_blank(), axis.title.x=element_blank())

tottenham_p <- ggplot(tottenham, aes(x = nb, y = place))+
  geom_point()+
  stat_smooth(se=FALSE, color='grey')+
  ylim(20,1)+
  ylab("Miejsce")+
  ggtitle("Tottenham")+
  theme_bw()+
  theme(plot.title = element_text(hjust=0.5), axis.text.x=element_blank(), axis.title.x=element_blank())
 
 
# at the end I put all plots in one 
  top_plot <- grid.arrange(arsenal_p,
             chelsea_p,
             liverpool_p,
             city_p,
             united_p,
             tottenham_p,
             ncol=3)
             
 # save plots
  ggsave("top six.png", plot = top_plot, scale = 1.5)
