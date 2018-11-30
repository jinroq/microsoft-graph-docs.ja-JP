---
title: メンバー
description: TeamsApp の現在のインストール状態を説明します。
ms.openlocfilehash: 7f358a621a25219e78e3a02ce081d07a27395d2c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072338"
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
