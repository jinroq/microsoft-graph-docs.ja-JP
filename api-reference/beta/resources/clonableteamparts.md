---
title: clonableTeamParts 列挙型
description: 'チームのどの部分のクローンを作成する必要があるについて説明します。 '
localization_priority: Normal
ms.openlocfilehash: 7eb71de266ea4f0ed9f94900dd03a47da1a24cc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860558"
---
# <a name="clonableteamparts-enum-type"></a>clonableTeamParts 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[チーム](../resources/team.md)のどの部分のクローンを作成する必要があるについて説明します。 

## <a name="members"></a>メンバー

| メンバー | 値| 説明 |
|:---------------|:--------|:----------|
|apps|1|インストールされたアプリの一覧をコピーします。|
|タブ|2|チャネル内のタブにコピーします。|
|settings|4|キーのグループの設定と、チーム内のすべての設定をコピーします。|
|チャンネル|8|チャネルの構造 (ただし、チャネル内のメッセージではない) をコピーします。|
|メンバー|16|メンバーとチームの所有者にコピーします。|
