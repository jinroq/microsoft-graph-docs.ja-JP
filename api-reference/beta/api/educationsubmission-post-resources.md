---
title: EducationSubmissionResource を作成します。
description: 'リソースを [リソース] リストに追加します。 このアクションは、この送信が割り当てられている受講者にのみ実行できます。 **AllowStudentsToAddResources**フラグが設定されていない場合、この操作は成功しません true に設定します。 呼び出し元は、ファイル ベースのリソースを新規作成する必要がある場合は、提出書類に関連付けられているリソース] フォルダーにファイルをアップロードする必要があります。 ファイルが存在しないか、そのフォルダーでは、POST 要求は失敗します。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a3c7592614eb1987df6730cd7f029bc84bb422cf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950649"
---
# <a name="create-educationsubmissionresource"></a>EducationSubmissionResource を作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

リソースを [リソース] リストに追加します。 このアクションは、この送信が割り当てられている受講者にのみ実行できます。 **AllowStudentsToAddResources**フラグが設定されていない場合、この操作は成功しません true に設定します。 呼び出し元は、ファイル ベースのリソースを新規作成する必要がある場合は、提出書類に関連付けられているリソース] フォルダーにファイルをアップロードする必要があります。 ファイルが存在しないか、そのフォルダーでは、POST 要求は失敗します。 

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。  |
|アプリケーション | サポートされていません。 | 

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/resources

```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
要求の本文には、 [educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトの JSON 表現を指定します。


## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文内の[educationSubmissionResource](../resources/educationsubmissionresource.md)オブジェクトです。

## <a name="example"></a>例
##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "ignored",
  "name": "create_educationsubmissionresource_from_educationsubmission"
}-->
```
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources
Content-type: application/json
Content-length: 1097

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
  "resource": {
      "@odata.type": "#microsoft.graph.educationWordResource",
      "displayName": "Report.docx",
      "createdDateTime": "2017-10-21T07:52:53.9863696Z",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
  },
  "@odata.type": "microsoft.graph.educationResource"
}

```

##### <a name="response"></a>応答
応答の例を次に示します。 

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 1152

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
  "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
  "resource": {
      "@odata.type": "#microsoft.graph.educationWordResource",
      "displayName": "Report.docx",
      "createdDateTime": "2017-10-21T07:52:53.9863696Z",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6",
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
