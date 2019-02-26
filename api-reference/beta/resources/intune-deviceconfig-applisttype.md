---
title: applisttype 列挙型
description: コンプライアンスアプリリストの可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b7d11107ca3ea2b698e28cd288f163ec190b0a6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172675"
---
# <a name="applisttype-enum-type"></a>applisttype 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

コンプライアンスアプリリストの可能な値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|既定値。意図的ではありません。|
|appsinlistcompliant|1-d|リストは、準拠していると見なされるアプリを表します (リスト上のアプリのみが準拠しています)。|
|appsnotinlistcompliant|pbm-2|このリストは、非準拠と見なされるアプリを表します (すべてのアプリはリスト上のアプリ以外に準拠しています)。|




