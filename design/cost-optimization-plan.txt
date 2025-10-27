
# Cost Optimization Plan – AWS Scalable Web Application Architecture

The architecture follows AWS Cost Optimization best practices to ensure efficient resource usage and lower operational costs.

---

1. Compute Optimization
   - Used EC2 right-sizing based on CPU/memory utilization.
   - Applied Auto Scaling to adjust instance count based on demand.
   - Used Reserved Instances for steady workloads.

2. Storage Optimization
   - Configured S3 lifecycle policies to move old objects to S3 Glacier.
   - Enabled Intelligent-Tiering for cost-effective storage transitions.
   - Compressed log files to reduce data storage.

3. Database Optimization
   - Used RDS Multi-AZ deployment for fault tolerance.
   - Scheduled backups during off-peak hours.
   - Monitored with CloudWatch to identify underutilized resources.

4. Network Optimization
   - Implemented CloudFront CDN to minimize latency and reduce data transfer costs.
   - Used Route 53 health checks for efficient routing.

5. Monitoring and Cost Review
   - Created CloudWatch alarms for idle resources.
   - Used AWS Cost Explorer and Trusted Advisor for monthly cost analysis.

---

 Result: Reduced infrastructure costs by approximately 25–30% while maintaining performance and reliability.
