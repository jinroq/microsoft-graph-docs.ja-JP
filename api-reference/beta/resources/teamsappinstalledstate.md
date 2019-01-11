---
title: メンバー
description: TeamsApp の現在のインストール状態を説明します。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 4e453a28b0c3ebc2957cf7e1a92a846e8e4758e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847573"
---
#<a name="teamsappinstalledstate-enum-type"></a>teamsAppInstalledState 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

の[teamsApp](teamsapp.md)の現在のインストール状態を説明します。

## <a name="members"></a>メンバー

| メンバー | 値| 説明 |
|:---------------|:--------|:----------|
|notInstalled|0|チームには、アプリケーションはインストールされていません。|
|インストールされています。|1|アプリケーションが正常にインストールします。|
|installedAndHidden|2|アプリケーションがインストールされているがビューから非表示にします。|
|installedAndPermanent|3|アプリケーションが完全にインストールされているしは削除できません。|
