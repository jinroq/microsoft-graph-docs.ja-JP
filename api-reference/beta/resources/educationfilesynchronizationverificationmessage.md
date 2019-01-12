---
title: educationFileSynchronizationVerificationMessage リソースの種類
description: CSV ベースの学校のデータのプロファイルの同期を開始する要求への応答としてクライアントに返されるエラーを表します。 リソースの検証エラーが含まれます。 ユーザーは Azure Active Directory (AD の Azure) との同期を要求を再起動する前にソース データを修正する必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: cda1d5d3ac56c50cdeb94ada091e8ae2975b8813
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914480"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>educationFileSynchronizationVerificationMessage リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

CSV ベースの学校のデータのプロファイルの[同期の開始](../api/educationsynchronizationprofile-start.md)を要求への応答としてクライアントに返されるエラーを表します。 リソースの検証エラーが含まれます。 ユーザーは Azure Active Directory (AD の Azure) との同期を要求を再起動する前にソース データを修正する必要があります。

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **type** | string | メッセージの種類です。 可能な値は、`error`、`warning`、`information` です。 | 
| **filename** | 文字列 | エラーを含むソース ファイルです。 |
| **description** | 文字列 | メッセージの種類に関する詳細な情報。 |

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
    "type": "String",
    "fileName": "String",
    "description": "String"
}
```
