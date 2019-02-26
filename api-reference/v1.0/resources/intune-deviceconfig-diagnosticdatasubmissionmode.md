---
title: diagnosticDataSubmissionMode 列挙型
description: デバイスが診断データと使用統計情報 (Watson など) を送信できるようにします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c0707b97e60da406210d6a091ed0dd4efaa2299
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251035"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスが診断データと使用統計情報 (Watson など) を送信できるようにします。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザーがを設定できるようにします。|
|none|1-d|テレメトリデータは、OS コンポーネントから送信されません。 注: この値は、エンタープライズおよびサーバーデバイスにのみ適用されます。 他のデバイスでこの設定を使用することは、値を1に設定するのと同じです。|
|基本的な|pbm-2|基本的なテレメトリデータを送信します。|
|保護|1/3|利用状況データおよびインサイトデータを含む、拡張されたテレメトリデータを送信します。|
|完全|2/4|システム状態などの診断データを含む完全なテレメトリデータを送信します。|



