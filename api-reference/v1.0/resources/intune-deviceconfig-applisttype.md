---
title: appListType 列挙型
description: コンプライアンスアプリリストの可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a02b8ed105206f53894ddb8d35dc24106eebebc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028603"
---
# <a name="applisttype-enum-type"></a>appListType 列挙型

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

コンプライアンスアプリリストの可能な値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|既定値。意図的ではありません。|
|appsInListCompliant|1-d|リストは、準拠していると見なされるアプリを表します (リスト上のアプリのみが準拠しています)。|
|appsNotInListCompliant|pbm-2|このリストは、非準拠と見なされるアプリを表します (すべてのアプリはリスト上のアプリ以外に準拠しています)。|



