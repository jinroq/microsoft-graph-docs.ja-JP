---
title: deviceEnrollmentType 列挙型
description: 管理するモバイル デバイスを追加するための方法です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 72acbdf412ebb91269fcdc3f851ffbc204e0274b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987756"
---
# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

管理するモバイル デバイスを追加するための方法です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|0|登録型の既定値は収集されませんでした。|
|userEnrollment|1|BYOD チャネルを通じてユーザー駆動の登録します。|
|deviceEnrollmentManager|2|デバイス登録の管理者アカウントとユーザー登録します。|
|appleBulkWithUser|3|アップル一括登録はユーザーのチャレンジ (DEP、Apple Configurator)。|
|appleBulkWithoutUser|4|ユーザーの課題 (DEP では、Apple の構成ウィザードは、モバイルの設定) にアップル一括登録します。|
|windowsAzureADJoin|5|Windows Azure AD を 10 に参加します。|
|windowsBulkUserless|6|証明書で ICD を Windows 10 一括登録します。|
|windowsAutoEnrollment|7|10 の Windows の自動登録します。 (勤務先のアカウントを追加)|
|windowsBulkAzureDomainJoin|8|10 の windows Azure AD に参加を一括します。|
|windowsCoManagement|9|Windows 10 共同管理が自動操縦装置、またはグループ ポリシーによって発生します。|



