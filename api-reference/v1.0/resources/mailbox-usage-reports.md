---
title: メールボックス使用状況レポート
description: メールボックス使用状況レポートを使用して、主に電子メールの送受信に基づき、メールボックスを持つユーザーの情報と、そのアクティビティのレベルを取得します。 また、各メールボックスが消費するストレージの量と、ストレージのクォータに近づいているメールボックスの数も確認できます。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: reports
ms.openlocfilehash: b018220f9f90577cfb6972528ae7013cc7f81fed
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919842"
---
# <a name="mailbox-usage-reports"></a>メールボックス使用状況レポート

メールボックス使用状況レポートを使用して、主に電子メールの送受信に基づき、メールボックスを持つユーザーの情報と、そのアクティビティのレベルを取得します。 また、各メールボックスが消費するストレージの量と、ストレージのクォータに近づいているメールボックスの数も確認できます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [メールボックスの詳細を取得する](../api/reportroot-getmailboxusagedetail.md) | Stream      | メールボックスの使用状況に関する詳細を取得します。         |
| [メールボックスの数を取得する](../api/reportroot-getmailboxusagemailboxcounts.md) | Stream      | 組織内のユーザー メールボックスの合計数と、レポート期間中の各日にアクティブなメールボックス数を取得します。 メールボックスは、ユーザーが何らかの電子メールを送信するか、読んだ場合にアクティブとみなされます。 |
| [クォータ状態のメールボックスの数を取得する](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | Stream      | 各クォータ カテゴリのユーザーのメールボックス数を取得します。 |
| [ストレージを取得する](../api/reportroot-getmailboxusagestorage.md) | Stream      | 組織で使用されているストレージの量を取得します。 |
