---
title: appListType 列挙型
description: コンプライアンスアプリリストの可能な値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b9166ef625387b47f07b56efd197dc22f1f440d0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333907"
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



