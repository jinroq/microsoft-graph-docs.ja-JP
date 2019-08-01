---
title: deviceEnrollmentType 列挙型
description: モバイルデバイスを管理に追加する方法には、次のようなものがあります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: afb007893ac0b41d4439635ed78b528058d41364
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036961"
---
# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 列挙型

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

モバイルデバイスを管理に追加する方法には、次のようなものがあります。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|既定値。登録の種類は収集されませんでした。|
|userEnrollment|1-d|BYOD channel 経由のユーザー主導型の登録。|
|deviceEnrollmentManager|pbm-2|デバイス登録マネージャーアカウントを使用したユーザー登録。|
|appleBulkWithUser|1/3|ユーザーチャレンジを使用した Apple 一括登録。 (DEP、Apple Configurator)|
|appleBulkWithoutUser|2/4|ユーザーチャレンジなしの Apple 一括登録。 (DEP、Apple Configurator、モバイル構成)|
|windowsAzureADJoin|5|Windows 10 Azure AD Join。|
|windowsBulkUserless|シックス|Windows 10 証明書を使用した ICD による一括登録。|
|windowsAutoEnrollment 登録|7|Windows 10 の自動登録。 (作業アカウントの追加)|
|windowsBulkAzureDomainJoin|8 |Windows 10 一括 Azure AD Join。|
|windowsCoManagement|9 |Windows 10 の共同管理は、自動操縦またはグループポリシーによって開始されます。|



