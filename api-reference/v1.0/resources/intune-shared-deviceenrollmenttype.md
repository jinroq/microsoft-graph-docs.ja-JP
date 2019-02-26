---
title: deviceEnrollmentType 列挙型
description: モバイルデバイスを管理に追加する方法には、次のようなものがあります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 62ff257e2f758776265f52a0d64cde52dbc26115
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261965"
---
# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

モバイルデバイスを管理に追加する方法には、次のようなものがあります。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|既定値。登録の種類は収集されませんでした。|
|userenrollment|1-d|byod channel 経由のユーザー主導型の登録。|
|deviceEnrollmentManager|pbm-2|デバイス登録マネージャーアカウントを使用したユーザー登録。|
|appleBulkWithUser|1/3|ユーザーチャレンジを使用した Apple 一括登録。 (DEP、Apple Configurator)|
|appleBulkWithoutUser|2/4|ユーザーチャレンジなしの Apple 一括登録。 (DEP、Apple Configurator、モバイル構成)|
|windowsAzureADJoin|5|Windows 10 Azure AD Join。|
|windowsbulkuserless|シックス|Windows 10 証明書を使用した ICD による一括登録。|
|windowsautoenrollment 登録|7|Windows 10 の自動登録。 (作業アカウントの追加)|
|windowsbulkazuredomainjoin|~|Windows 10 一括 Azure AD Join。|
|windowsCoManagement|i-9|Windows 10 の共同管理は、自動操縦またはグループポリシーによって開始されます。|



