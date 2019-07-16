---
title: userPfxIntendedPurpose 列挙型
description: ユーザー PFX 証明書の目的のためにサポートされている値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1790b1d1835d19cacb7e3b32262ce06be4daa378
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739282"
---
# <a name="userpfxintendedpurpose-enum-type"></a>userPfxIntendedPurpose 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ユーザー PFX 証明書の目的のためにサポートされている値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|未定義|.0|役割/使用状況は割り当てられていません。|
|smimeEncryption|1-d|S/MIME 暗号化に対して有効です。|
|smimeSigning|pbm-2|S/MIME 署名に対して有効です。|
|仮想|2/4|VPN で使用する場合に有効です。|
|wi-fi|8 |WiFi で使用するのに有効です。|





