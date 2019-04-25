---
title: deviceEnrollmentType 列挙型
description: モバイルデバイスを管理に追加する方法には、次のようなものがあります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b186110c4f69ea7b6f4d12c9fb2a333927f81385
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524590"
---
# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

モバイルデバイスを管理に追加する方法には、次のようなものがあります。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|既定値。登録の種類は収集されませんでした。|
|userenrollment|1 |byod channel 経由のユーザー主導型の登録。|
|deviceEnrollmentManager|2 |デバイス登録マネージャーアカウントを使用したユーザー登録。|
|appleBulkWithUser|3 |ユーザーチャレンジを使用した Apple 一括登録。 (DEP、Apple Configurator)|
|appleBulkWithoutUser|4 |ユーザーチャレンジなしの Apple 一括登録。 (DEP、Apple Configurator、モバイル構成)|
|windowsAzureADJoin|5 |Windows 10 Azure AD Join。|
|windowsbulkuserless|6 |Windows 10 証明書を使用した ICD による一括登録。|
|windowsautoenrollment 登録|7 |Windows 10 の自動登録。 (作業アカウントの追加)|
|windowsbulkazuredomainjoin|8 |Windows 10 一括 Azure AD Join。|
|windowsCoManagement|9 |Windows 10 の共同管理は、自動操縦またはグループポリシーによって開始されます。|




