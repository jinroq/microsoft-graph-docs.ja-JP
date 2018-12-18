---
title: Members
description: TeamsApp の現在のインストール状態を説明します。
author: nkramer
ms.openlocfilehash: a73c68298c4cdf65deee68fb3bd707d50bc2475a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316794"
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
