---
title: eapFastConfiguration 列挙型
description: EAP-FAST 構成の使用可能な設定です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fa2c3c3a4cf0bc245ea7c9fbc4294d69215deee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399389"
---
# <a name="eapfastconfiguration-enum-type"></a>eapFastConfiguration 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

EAP-FAST 構成の使用可能な設定です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noProtectedAccessCredential|0|EAP-FAST クリデンシャル (PAC) の保護されたアクセスなしを使用します。|
|useProtectedAccessCredential|1|保護されたアクセス クリデンシャル (PAC) をを利用します。|
|useProtectedAccessCredentialAndProvision|2|使用してアクセスを保護するクリデンシャル (PAC) と PAC. を提供します。|
|useProtectedAccessCredentialAndProvisionAnonymously|3|保護されたアクセスの資格情報 (PAC)、PAC のプロビジョニングを使用して実行し、匿名で。|




