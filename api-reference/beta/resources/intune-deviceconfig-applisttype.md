---
title: appListType 列挙型
description: コンプライアンスアプリリストの可能な値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5df56b14d3c5416a04245ffbccd0b3b887266bde
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987790"
---
# <a name="applisttype-enum-type"></a>appListType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

コンプライアンスアプリリストの可能な値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|既定値。意図的ではありません。|
|appsInListCompliant|1-d|リストは、準拠していると見なされるアプリを表します (リスト上のアプリのみが準拠しています)。|
|appsNotInListCompliant|pbm-2|このリストは、非準拠と見なされるアプリを表します (すべてのアプリはリスト上のアプリ以外に準拠しています)。|





