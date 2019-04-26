---
title: メール アプリ使用状況レポート
description: メール アプリの使用状況レポートを使用して、Exchange Online に接続するために使用されたメール アプリの数を確認します。 また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 00adbec446cda1ea6855c7f52e847f88f42c65bd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555900"
---
# <a name="email-app-usage-reports"></a>メール アプリ使用状況レポート

メール アプリの使用状況レポートを使用して、Exchange Online に接続するために使用されたメール アプリの数を確認します。 また、サポート対象の Outlook バージョンにアップグレードする必要のあるユーザーをフォローアップするために、どの Outlook アプリのバージョンが使用されているかも確認できます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メール アプリの使用状況](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getemailappusageuserdetail.md) | ストリーム      | メール アプリの各バージョンでユーザーが実行したアクティビティの詳細を取得します。 |
| [アプリのユーザーの数を取得する](../api/reportroot-getemailappusageappsusercounts.md) | Stream      | メール アプリごとの、それぞれ別個のユーザーの数を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getemailappusageusercounts.md) | Stream      | 任意のメール アプリを使用して Exchange Online に接続されている、それぞれ別個のユーザー数を取得します。 |
| [バージョンのユーザーの数を取得する](../api/reportroot-getemailappusageversionsusercounts.md) | Stream      | Outlook デスクトップ版ごとの、それぞれ別個のユーザー数を取得します。 |
