---
title: secureAssessmentAccountType 列挙型
description: Windows10SecureAssessment ConfigurationAccount で許可されているアカウントの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ff967766321b5e7be5dd33944a02e4ed2bdc280
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986649"
---
# <a name="secureassessmentaccounttype-enum-type"></a>secureAssessmentAccountType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows10SecureAssessment ConfigurationAccount で許可されているアカウントの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|azureADAccount|.0|Azure AD アカウントが AzureAD\username@tenant.com の形式であることを示します。|
|domainAccount|1-d|ドメインアカウントが domain\user または user@domain.com の形式であることを示します。|
|localAccount|pbm-2|ユーザー名の形式でローカルアカウントを示します。|





