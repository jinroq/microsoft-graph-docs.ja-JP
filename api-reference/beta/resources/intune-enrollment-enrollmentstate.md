---
title: enrollmentState 列挙型
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4f394b02eac7e54c7e74a1c6954d6e3a7414e1b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999186"
---
# <a name="enrollmentstate-enum-type"></a>enrollmentState 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|デバイス登録の状態が不明です|
|遂げ|1-d|デバイスは登録されています。|
|pendingReset|pbm-2|登録済みですが、登録プロファイルによって登録され、登録されたプロファイルは割り当てられたプロファイルとは異なります。|
|フェール|1/3|登録されていません。登録エラーレコードがあります。|
|notContacted|2/4|デバイスはインポートされていますが、登録されていません。|
|ブロック|5|デバイスは userless として登録されていますが、アプリのインストールが失敗したため、ユーザー登録への移動がブロックされています。|





