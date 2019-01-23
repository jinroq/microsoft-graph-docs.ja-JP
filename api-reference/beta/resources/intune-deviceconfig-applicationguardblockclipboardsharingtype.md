---
title: applicationGuardBlockClipboardSharingType 列挙型
description: ApplicationGuardBlockClipboardSharingType に指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f9621db53e16231f710cccb12d79f65d22d4017
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415062"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a>applicationGuardBlockClipboardSharingType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ApplicationGuardBlockClipboardSharingType に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|構成されていません|
|blockBoth|1|ブロックのクリップボード データのコンテナーにホストとホスト コンテナーの両方を共有するには|
|blockHostToContainer|2|コンテナーにホストからのデータを共有するためのブロックのクリップボード|
|blockContainerToHost|3|コンテナーからホストへのデータを共有するためのブロックのクリップボード|
|blockNone|4|ブロックのクリップボード データのコンテナーにホストもホストするためのコンテナーを共有するには|




