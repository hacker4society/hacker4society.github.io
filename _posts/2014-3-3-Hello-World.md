---
layout: post
title: You're up and running!
published: true
---
#This is my first post
    	package myinterface;
interface Geoanalyzer {
	final static float pi = 3.142f;
	float area();
	float perimeter();
}
class circle implements Geoanalyzer {
	float radius;
	circle (float r){
		radius = r;
	}
	public float area(){
		return(pi*radius*radius);
	}
	public float perimeter(){
		return(2*pi*radius);
	}
}

