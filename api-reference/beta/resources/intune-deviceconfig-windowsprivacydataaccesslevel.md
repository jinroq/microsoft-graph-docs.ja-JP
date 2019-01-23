---
title: windowsPrivacyDataAccessLevel 列挙型
description: Windows プライバシー データの特定のカテゴリへのアクセス レベルを決定します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5d6fed0897b22a6a6b478dc5d2b7954faca42b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410624"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>windowsPrivacyDataAccessLevel 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows プライバシー データの特定のカテゴリへのアクセス レベルを決定します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|目的なしアクセス レベルが指定されませんでした。 デバイスは、UserInControl や ForceAllow のように動作可能性があります。 プライバシー ・ データによりますが、されたバージョンの Windows およびその他の要素にアクセスします。|
|forceAllow|1|アプリケーションは、指定したプライバシー データへのアクセスが許可されます。|
|forceDeny|2|指定したプライバシー ・ データにアクセスするアプリケーションは拒否されます。|
|userInControl|3|アプリケーションが指定したプライバシー ・ データにアクセスしようとした場合、ユーザーが要求されます。|




