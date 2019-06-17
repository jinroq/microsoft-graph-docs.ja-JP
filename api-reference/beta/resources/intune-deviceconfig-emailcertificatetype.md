---
title: emailCertificateType 列挙型
description: 電子メールの署名と暗号化に対してサポートされている証明書ソース。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2ff58f55033660a839a5f28d0244217c62936e0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996388"
---
# <a name="emailcertificatetype-enum-type"></a>emailCertificateType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

電子メールの署名と暗号化に対してサポートされている証明書ソース。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|証明書をソースとして使用しないでください。|
|certificate|1-d|証明書ソースに証明書を使用します。|
|derivedCredential|pbm-2|証明書ソースに派生した資格情報を使用します。|





