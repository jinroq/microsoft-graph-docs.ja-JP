---
title: secureAssessmentAccountType 列挙型
description: Windows10SecureAssessment configurationaccount で許可されているアカウントの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fa14d90465ed9278fd20362800d5d111de62950
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464944"
---
# <a name="secureassessmentaccounttype-enum-type"></a>secureAssessmentAccountType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows10SecureAssessment configurationaccount で許可されているアカウントの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|azureADAccount|.0|Azure AD アカウントが AzureAD\username@tenant.com の形式であることを示します。|
|domainaccount|1-d|ドメインアカウントが domain\user または user@domain.com の形式であることを示します。|
|localaccount|pbm-2|ユーザー名の形式でローカルアカウントを示します。|





