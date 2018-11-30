---
title: clonableTeamParts 列挙型
description: 'チームのどの部分のクローンを作成する必要があるについて説明します。 '
ms.openlocfilehash: 123cdb5ff7fd4a4291df5d9352b0db466908cc3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067813"
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
