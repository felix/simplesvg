# Makefile for a PyQGIS plugin 
UI_FILES = Ui_SimpleSvg.py mapsizer/Ui_MapSizer.py

RESOURCE_FILES = resources.py

default: compile
	
compile: $(UI_FILES) $(RESOURCE_FILES)

%.py : %.qrc
	pyrcc4 -o $@ $<

%.py : %.ui
	pyuic4 -o $@ $<

