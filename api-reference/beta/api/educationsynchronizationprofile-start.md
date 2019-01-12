---
title: EducationSynchronizationProfile にファイルをアップロードした後に同期を開始します。
description: テナントで特定の学校のデータの同期プロファイルをファイルのアップロードを確認します。 検証が成功した場合は、プロファイルの同期が開始されます。 それ以外の場合、エラーおよび警告の応答が含まれます。 応答にエラーが含まれている場合、同期は開始されません。 応答には、警告のみが含まれている場合、は、同期が開始されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: efdc0863a1de58f7ebf46492b662e632972275c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915250"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a>EducationSynchronizationProfile にファイルをアップロードした後に同期を開始します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

テナント内の特定の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)にファイルがアップロードされたことを確認します。 検証が成功した場合は、プロファイルの同期が開始されます。 それ以外の場合、エラーおよび警告の応答が含まれます。 応答にエラーが含まれている場合、同期は開始されません。 応答には、警告のみが含まれている場合、は、同期が開始されます。

> **注:** データ プロバイダーが型[educationcsvdataprovider](../resources/educationcsvdataprovider.md)の場合にのみ、このメソッドを使用します。 また、プロファイルの状態プロパティは、開始する前に準備する必要があります。 State プロパティを確認するには、そのプロファイル オブジェクトをポーリングします。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類 | Permissions |
|:-----------|:----------|
| 委任 (職場または学校のアカウント) | EduAdministration.ReadWrite |
|(個人用の Microsoft アカウントを委任します。|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 種類 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。
## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードを返します。 失敗した場合、返されます、 `400 Bad Request`。 応答には、エラーや警告が検出された場合、応答の本体の一部として[educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md)オブジェクトのコレクションが含まれています。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```

##### <a name="response"></a>応答
以下は、応答の例です。 

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2105

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/Collection(microsoft.graph.verificationMessage)",
    "value": [
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have missing data for the field - SIS ID"
        },
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have an invalid format for the field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "125 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "35 row(s) have referenced data not found in source. Field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "10 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "91 row(s) have referenced data not found in source. Field - SIS ID"
        }
    ]
}
```
