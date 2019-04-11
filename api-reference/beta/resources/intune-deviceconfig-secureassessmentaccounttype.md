---
title: secureAssessmentAccountType 列挙型
description: Windows10SecureAssessment configurationaccount で許可されているアカウントの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fa14d90465ed9278fd20362800d5d111de62950
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795010"
---
# <a name="secureassessmentaccounttype-enum-type"></a>secureAssessmentAccountType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows10SecureAssessment configurationaccount で許可されているアカウントの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|azureADAccount|.0|Azure AD アカウントがのAzureAD\username@tenant.com形式であることを示します。|
|domainaccount|1-d|ドメインアカウントが domain\user またはuser@domain.comの形式であることを示します。|
|localaccount|pbm-2|ユーザー名の形式でローカルアカウントを示します。|





