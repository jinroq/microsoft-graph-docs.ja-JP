---
title: eapFastConfiguration 列挙型
description: EAP-FAST 構成で利用可能な設定。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8deeae69bb4d828cc2e0178c79aba200f8a4709e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946813"
---
# <a name="eapfastconfiguration-enum-type"></a>eapFastConfiguration 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

EAP-FAST 構成で利用可能な設定。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noProtectedAccessCredential|.0|保護されたアクセス資格情報 (PAC) を使用せずに、EAP-FAST を使用します。|
|useProtectedAccessCredential|1-d|保護されたアクセス資格情報 (PAC) を使用します。|
|useProtectedAccessCredentialAndProvision|pbm-2|保護されたアクセス資格情報 (PAC) を使用し、PAC をプロビジョニングします。|
|useProtectedAccessCredentialAndProvisionAnonymously|1/3|保護されたアクセス資格情報 (PAC) を使用し、PAC をプロビジョニングして、匿名で行います。|




