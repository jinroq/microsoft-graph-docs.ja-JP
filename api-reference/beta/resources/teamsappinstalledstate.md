---
title: メンバー
description: TeamsApp の現在のインストール状態を説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ca42b56e2c374dbaea1df676e3a84569b192e78c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937174"
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
