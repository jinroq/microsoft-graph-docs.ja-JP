---
title: appListType 列挙型
description: 準拠のアプリケーションのリストで使用できる値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf8930136b00b7b5579ec5e7266b6a77a9a11968
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415223"
---
# <a name="applisttype-enum-type"></a>appListType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

準拠のアプリケーションのリストで使用できる値です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|既定値でことを目的しません。|
|appsInListCompliant|1|一覧は、考慮される準拠 (準拠では、リスト上のアプリ) 専用のアプリケーションを表します。|
|appsNotInListCompliant|2|リストと見なされます非準拠のアプリケーションを表します (すべてのアプリケーション準拠では、リスト上のアプリを除く)。|




