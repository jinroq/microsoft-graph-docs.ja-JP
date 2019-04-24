---
title: Office 365 アクティブ化レポート
description: Office 365 アクティブ化レポートでは、1 つ以上のデバイスで Office 365 サブスクリプションをアクティブ化したユーザーが表示されます。 これらのレポートでは、Office 365 ProPlus、Project、Visio Pro for Office 365 のサブスクリプションのアクティブ化の詳細、およびデスクトップとデバイス全体にわたるアクティブ化の詳細を確認できます。 これらのレポートは、Office サブスクリプションをアクティブ化するために追加サポートが必要なユーザーの識別に役立ちます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 44775b2a14bbd00452d27a04f8e225612100b3fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463055"
---
# <a name="office-365-activations-reports"></a>Office 365 アクティブ化レポート

Office 365 アクティブ化レポートでは、1 つ以上のデバイスで Office 365 サブスクリプションをアクティブ化したユーザーが表示されます。 これらのレポートでは、Office 365 ProPlus、Project、Visio Pro for Office 365 のサブスクリプションのアクティブ化の詳細、およびデスクトップとデバイス全体にわたるアクティブ化の詳細を確認できます。 これらのレポートは、Office サブスクリプションをアクティブ化するために追加サポートが必要なユーザーの識別に役立ちます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。

## <a name="reports"></a>レポート
| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getoffice365activationsuserdetail.md) | Stream      | Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。 |
| [ライセンス認証の数を取得する](../api/reportroot-getoffice365activationcounts.md) | Stream      | デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getoffice365activationsusercounts.md) | Stream      | 有効なユーザーで、デスクトップまたはデバイスで Office サブスクリプションがアクティブ化されているユーザーの数を取得します。 |
