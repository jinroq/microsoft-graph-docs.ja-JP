---
title: emailCertificateType 列挙型
description: 電子メールの署名と暗号化に対してサポートされている証明書ソース。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c6c4a6943fada88dc9a30c9e81d45705153dfde1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357188"
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



