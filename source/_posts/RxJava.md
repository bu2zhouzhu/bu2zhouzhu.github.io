---
title: RxJava
date: 2016-11-25 16:38:08
tags:
---
Observable.create方法中对 subscriber 执行 onNext 和 onComplete 前, 需要先判断 subscriber.isUnsubscribed().
Subject 执行 onNext 前则不需要做这个判断(也无法判断), 证明了 Subject是 hot observable.
