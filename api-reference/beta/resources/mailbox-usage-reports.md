---
title: メールボックス使用状況レポート
description: メールボックスと、主に電子メールの送受信に基づくアクティビティレベルのユーザーに関する情報を取得できます。 また、各メールボックスが消費するストレージの量と、ストレージのクォータに近づいているメールボックスの数も確認できます。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: ae0b3294750271f32d91dca79f75e7cf44641045
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463531"
---
# <a name="mailbox-usage-reports"></a>メールボックス使用状況レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

メールボックスと、主に電子メールの送受信に基づくアクティビティレベルのユーザーに関する情報を取得できます。 また、各メールボックスが消費するストレージの量と、ストレージのクォータに近づいているメールボックスの数も確認できます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: メールボックスの使用状況](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV 戻り値の型 | JSON 戻り値の種類                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [メールボックスの詳細を取得する](../api/reportroot-getmailboxusagedetail.md) | Stream          | [mailboxUsageDetail](../resources/mailboxusagedetail.md) | メールボックスの使用状況に関する詳細を取得します。         |
| [メールボックスの数を取得する](../api/reportroot-getmailboxusagemailboxcounts.md) | Stream          | [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) | 組織内のユーザー メールボックスの合計数と、レポート期間中の各日にアクティブなメールボックス数を取得します。 メールボックスは、ユーザーが何らかの電子メールを送信するか、読んだ場合にアクティブとみなされます。 |
| [クォータ状態のメールボックスの数を取得する](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | Stream          | [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) | 各クォータ カテゴリのユーザーのメールボックス数を取得します。 |
| [ストレージを取得する](../api/reportroot-getmailboxusagestorage.md) | Stream          | [mailboxUsageStorage](../resources/mailboxusagestorage.md) | 組織で使用されているストレージの量を取得します。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailbox-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
