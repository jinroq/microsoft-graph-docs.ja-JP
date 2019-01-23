---
title: appLogUploadState 列挙型
description: AppLogUploadStatus
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 58dcc0d4a15370d6449772d917e8994f0eb9e7bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431666"
---
# <a name="apploguploadstate-enum-type"></a>appLogUploadState 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

AppLogUploadStatus

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|保留中|0|要求が処理を待機しているかの処理|
|完了|1|ダウンロードの Azure blob にアップロードされたファイルを使用して要求を完了するとします。|
|失敗しました。|2|要求は、処理し、エラー状態で終了しました。|




