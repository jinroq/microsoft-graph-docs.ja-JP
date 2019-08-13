---
title: deviceManagementExchangeAccessLevel 列挙型
description: Exchange のアクセスレベル。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f1059706429c566c672e09a95a291c24a1760181
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374233"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a>deviceManagementExchangeAccessLevel 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Exchange のアクセスレベル。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|Exchange でデバイスアクセスルールが構成されていません。|
|使う|1-d|デバイスへのアクセスを Exchange に許可します。|
|拒否|pbm-2|デバイスによる Exchange へのアクセスをブロックします。|
|済み|1/3|Exchange でデバイスを検疫します。|



