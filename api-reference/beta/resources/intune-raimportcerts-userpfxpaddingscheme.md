---
title: Userpfxps/スキーム列挙型
description: 暗号化プロバイダーで使用される埋め込み方式のサポートされている値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a079075d3e0a44a773c854df55df1635d54584c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739275"
---
# <a name="userpfxpaddingscheme-enum-type"></a>Userpfxps/スキーム列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

暗号化プロバイダーで使用される埋め込み方式のサポートされている値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|パディングを使用しません。|
|pkcs1|1-d|PKCS # 1 のパディングを使用します。|
|oaepSha1|pbm-2|OAEP のパディングを使用します。|
|oaepSha256|1/3|OAEP 256 のパディングを使用します。|
|oaepSha384|2/4|OAEP 384 のパディングを使用します。|
|oaepSha512|5|OAEP 512 のパディングを使用します。|





