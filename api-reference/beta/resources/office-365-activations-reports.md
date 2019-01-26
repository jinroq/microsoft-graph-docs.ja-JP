---
title: Office 365 アクティブ化レポート
description: Office 365 のライセンス認証のレポートを使用すると、ユーザー先のデバイスが少なくとも 1 つの Office 365 サブスクリプションを有効にして表示します。 デスクトップとデバイスの間でのアクティブ化の詳細と、Office 365 サブスクリプションのライセンス認証を Office 365 用リソース、プロジェクト、および Visio Pro の内訳を提供します。 このレポートを使用すると可能性があります、Office のサブスクリプションをアクティブにするのには追加のサポートを必要とするユーザーを識別できます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 345ab500ef5986471bb801a88ee5886473a3dd60
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573679"
---
# <a name="office-365-activations-reports"></a>Office 365 アクティブ化レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Office 365 のライセンス認証のレポートを使用すると、ユーザー先のデバイスが少なくとも 1 つの Office 365 サブスクリプションを有効にして表示します。 デスクトップとデバイスの間でのアクティブ化の詳細と、Office 365 サブスクリプションのライセンス認証を Office 365 用リソース、プロジェクト、および Visio Pro の内訳を提供します。 このレポートを使用すると可能性があります、Office のサブスクリプションをアクティブにするのには追加のサポートを必要とするユーザーを識別できます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。

## <a name="reports"></a>レポート
| 関数                                 | CSV の戻り値の型 | JSON の戻り値の型                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getoffice365activationsuserdetail.md) | Stream          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。 |
| [ライセンス認証の数を取得する](../api/reportroot-getoffice365activationcounts.md) | Stream          | [office365ActivationCounts](../resources/office365activationcounts.md) | デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getoffice365activationsusercounts.md) | Stream          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | 有効なユーザーで、デスクトップまたはデバイスで Office サブスクリプションがアクティブ化されているユーザーの数を取得します。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-activations-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
