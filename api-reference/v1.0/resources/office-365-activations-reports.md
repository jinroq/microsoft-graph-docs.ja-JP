---
title: Office 365 アクティブ化レポート
description: Office 365 アクティブ化レポートでは、1 つ以上のデバイスで Office 365 サブスクリプションをアクティブ化したユーザーが表示されます。 これらのレポートでは、Office 365 ProPlus、Project、Visio Pro for Office 365 のサブスクリプションのアクティブ化の詳細、およびデスクトップとデバイス全体にわたるアクティブ化の詳細を確認できます。 これらのレポートは、Office サブスクリプションをアクティブ化するために追加サポートが必要なユーザーの識別に役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 5ecf1aeb0014ec8ead97fc7d1b01d366c9565291
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035988"
---
# <a name="office-365-activations-reports"></a>Office 365 アクティブ化レポート

Office 365 アクティブ化レポートでは、1 つ以上のデバイスで Office 365 サブスクリプションをアクティブ化したユーザーが表示されます。 これらのレポートでは、Office 365 ProPlus、Project、Visio Pro for Office 365 のサブスクリプションのアクティブ化の詳細、およびデスクトップとデバイス全体にわたるアクティブ化の詳細を確認できます。 これらのレポートは、Office サブスクリプションをアクティブ化するために追加サポートが必要なユーザーの識別に役立ちます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。

## <a name="reports"></a>レポート
| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getoffice365activationsuserdetail.md) | ストリーム      | Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。 |
| [ライセンス認証の数を取得する](../api/reportroot-getoffice365activationcounts.md) | Stream      | デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getoffice365activationsusercounts.md) | Stream      | 有効なユーザーで、デスクトップまたはデバイスで Office サブスクリプションがアクティブ化されているユーザーの数を取得します。 |
