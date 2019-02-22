---
title: enrollmentState 列挙型
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcb039563d9c45a33c4e42344fc8557dfe29b333
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159249"
---
# <a name="enrollmentstate-enum-type"></a>enrollmentState 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|デバイス登録の状態が不明です|
|遂げ|1-d|デバイスは登録されています。|
|pendingreset|pbm-2|登録済みですが、登録プロファイルによって登録され、登録されたプロファイルは割り当てられたプロファイルとは異なります。|
|フェール|1/3|登録されていません。登録エラーレコードがあります。|
|notcontacted|2/4|デバイスはインポートされていますが、登録されていません。|
|ブロック|5|デバイスは userless として登録されていますが、アプリのインストールが失敗したため、ユーザー登録への移動がブロックされています。|




