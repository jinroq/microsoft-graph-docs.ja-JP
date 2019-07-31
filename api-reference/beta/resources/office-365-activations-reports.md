---
title: Office 365 アクティブ化レポート
description: Office 365 アクティブ化レポートには、少なくとも1つのデバイスで Office 365 サブスクリプションをアクティブ化したユーザーが表示されます。 これにより、Office 365 ProPlus、Project、および Visio Pro for Office 365 サブスクリプションのライセンス認証の内訳に加え、デスクトップとデバイス間でのライセンス認証の内訳が提供されます。 このレポートは、Office サブスクリプションのライセンス認証を行うために追加のサポートが必要になる可能性があるユーザーを特定するのに役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 1e3a3831c3ea5c2b4307ae612630421365992759
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009553"
---
# <a name="office-365-activations-reports"></a>Office 365 アクティブ化レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Office 365 アクティブ化レポートには、少なくとも1つのデバイスで Office 365 サブスクリプションをアクティブ化したユーザーが表示されます。 これにより、Office 365 ProPlus、Project、および Visio Pro for Office 365 サブスクリプションのライセンス認証の内訳に加え、デスクトップとデバイス間でのライセンス認証の内訳が提供されます。 このレポートは、Office サブスクリプションのライセンス認証を行うために追加のサポートが必要になる可能性があるユーザーを特定するのに役立ちます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。

## <a name="reports"></a>レポート
| 関数                                 | CSV 戻り値の型 | JSON 戻り値の種類                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getoffice365activationsuserdetail.md) | ストリーム          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。 |
| [ライセンス認証の数を取得する](../api/reportroot-getoffice365activationcounts.md) | Stream          | [office365ActivationCounts](../resources/office365activationcounts.md) | デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getoffice365activationsusercounts.md) | Stream          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | 有効なユーザーで、デスクトップまたはデバイスで Office サブスクリプションがアクティブ化されているユーザーの数を取得します。 |
