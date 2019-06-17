---
title: diagnosticDataSubmissionMode 列挙型
description: デバイスが診断データと使用統計情報 (Watson など) を送信できるようにします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf69232ee31bf7fd1eebd440e482d76c052f4fbc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989925"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスが診断データと使用統計情報 (Watson など) を送信できるようにします。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザーがを設定できるようにします。|
|none|1-d|テレメトリデータは、OS コンポーネントから送信されません。 注: この値は、エンタープライズおよびサーバーデバイスにのみ適用されます。 他のデバイスでこの設定を使用することは、値を1に設定するのと同じです。|
|基本的な|pbm-2|基本的なテレメトリデータを送信します。|
|保護|1/3|利用状況データおよびインサイトデータを含む、拡張されたテレメトリデータを送信します。|
|完全|2/4|システム状態などの診断データを含む完全なテレメトリデータを送信します。|





