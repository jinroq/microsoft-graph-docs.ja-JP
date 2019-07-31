---
title: vppTokenState 列挙型
description: Apple Volume Purchase Program のトークンに関連付けられている状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d9ae2b3bfb45ff33c5f0a39d746350212db3027c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010638"
---
# <a name="vpptokenstate-enum-type"></a>vppTokenState 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Apple Volume Purchase Program のトークンに関連付けられている状態。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|既定の状態です。|
|有効な|1-d|トークンが有効です。|
|終了|pbm-2|トークンの有効期限が切れています。|
|無効です|1/3|トークンが無効です。|
|assignedToExternalMDM|2/4|トークンは別の MDM サービスによって管理されています。|





