---
title: eapfastconfiguration 列挙型
description: eap-fast 構成で利用可能な設定。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0d8a250b2272ae8b8287f9869697633493b116f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173571"
---
# <a name="eapfastconfiguration-enum-type"></a>eapfastconfiguration 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

eap-fast 構成で利用可能な設定。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noProtectedAccessCredential|.0|保護されたアクセス資格情報 (PAC) を使用せずに、eap-fast を使用します。|
|useProtectedAccessCredential|1-d|保護されたアクセス資格情報 (PAC) を使用します。|
|useProtectedAccessCredentialAndProvision|pbm-2|保護されたアクセス資格情報 (pac) を使用し、pac をプロビジョニングします。|
|useProtectedAccessCredentialAndProvisionAnonymously|1/3|保護されたアクセス資格情報 (pac) を使用し、pac をプロビジョニングして、匿名で行います。|




