---
title: folderProtectionType 列挙型
description: フォルダーの保護の使用可能な値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e2abbb719ab93b53ad276f8391d4028c4f8b40b4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405717"
---
# <a name="folderprotectiontype-enum-type"></a>folderProtectionType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

フォルダーの保護の使用可能な値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|デバイスの既定値でことを目的しません。|
|有効にします。|1|機能をブロックします。|
|auditMode|2|機能を許可するが、ログを生成します。|
|blockDiskModification|3|ディスク ・ セクターへの書き込みから信頼されていないアプリケーションをブロックします。|
|auditDiskModification|4|信頼されていないアプリケーションがディスクのセクターに書き込むときは、ログを生成します。|




