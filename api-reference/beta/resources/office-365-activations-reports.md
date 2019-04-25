---
title: Office 365 アクティブ化レポート
description: office 365 アクティブ化レポートには、少なくとも1つのデバイスで office 365 サブスクリプションをアクティブ化したユーザーが表示されます。 これにより、office 365 ProPlus、Project、および Visio Pro for office 365 サブスクリプションのライセンス認証の内訳に加え、デスクトップとデバイス間でのライセンス認証の内訳が提供されます。 このレポートは、Office サブスクリプションのライセンス認証を行うために追加のサポートが必要になる可能性があるユーザーを特定するのに役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 345ab500ef5986471bb801a88ee5886473a3dd60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581593"
---
# <a name="office-365-activations-reports"></a>Office 365 アクティブ化レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

office 365 アクティブ化レポートには、少なくとも1つのデバイスで office 365 サブスクリプションをアクティブ化したユーザーが表示されます。 これにより、office 365 ProPlus、Project、および Visio Pro for office 365 サブスクリプションのライセンス認証の内訳に加え、デスクトップとデバイス間でのライセンス認証の内訳が提供されます。 このレポートは、Office サブスクリプションのライセンス認証を行うために追加のサポートが必要になる可能性があるユーザーを特定するのに役立ちます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。

## <a name="reports"></a>レポート
| 関数                                 | CSV 戻り値の型 | JSON 戻り値の種類                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getoffice365activationsuserdetail.md) | ストリーム          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。 |
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
