---
title: Office 365 アクティブ化レポート
description: Office 365 のライセンス認証のレポートを使用すると、ユーザー先のデバイスが少なくとも 1 つの Office 365 サブスクリプションを有効にして表示します。 デスクトップとデバイスの間でのアクティブ化の詳細と、Office 365 サブスクリプションのライセンス認証を Office 365 用リソース、プロジェクト、および Visio Pro の内訳を提供します。 このレポートを使用すると可能性があります、Office のサブスクリプションをアクティブにするのには追加のサポートを必要とするユーザーを識別できます。
ms.openlocfilehash: 745ca24de47f576522f2f81e3f9d7b70921d81ea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073108"
---
# <a name="office-365-activations-reports"></a>Office 365 アクティブ化レポート

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Office 365 のライセンス認証のレポートを使用すると、ユーザー先のデバイスが少なくとも 1 つの Office 365 サブスクリプションを有効にして表示します。 デスクトップとデバイスの間でのアクティブ化の詳細と、Office 365 サブスクリプションのライセンス認証を Office 365 用リソース、プロジェクト、および Visio Pro の内訳を提供します。 このレポートを使用すると可能性があります、Office のサブスクリプションをアクティブにするのには追加のサポートを必要とするユーザーを識別できます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)」を参照してください。

## <a name="reports"></a>レポート
| 関数                                 | CSV の戻り値の型 | JSON の戻り値の型                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getoffice365activationsuserdetail.md) | Stream          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。 |
| [ライセンス認証の数を取得する](../api/reportroot-getoffice365activationcounts.md) | Stream          | [office365ActivationCounts](../resources/office365activationcounts.md) | デスクトップとデバイスでの Office 365 のライセンス認証の数を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getoffice365activationsusercounts.md) | Stream          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | 有効なユーザーで、デスクトップまたはデバイスで Office サブスクリプションがアクティブ化されているユーザーの数を取得します。 |
