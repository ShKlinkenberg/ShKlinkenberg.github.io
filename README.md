# Personal website

install.packages("blogdown")

blogdown::install_hugo(version = 0.44, use_brew = FALSE, force = TRUE)

blogdown::build_site()
blogdown::serve_site()

servr::daemon_stop(1)